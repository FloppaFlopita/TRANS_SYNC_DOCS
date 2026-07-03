# 📄 ADR 001: Arquitectura de Monolito Modular para el Sistema TRANS-SYNC

**Estado:** Aceptado  
**Fecha:** 2026-07-02  
**Autores:** Equipo de Desarrollo Synergy6  

## 1. Contexto y Problema
La empresa **Transportes Veloz Altiplano E.I.R.L.** requiere un ecosistema digital ("TRANS-SYNC") para sincronizar sus operaciones entre las sedes de Juliaca, Puno y Cusco, y las unidades móviles en ruta. El negocio sufre pérdidas económicas por la sobreventa de asientos, descontrol de caja y falta de trazabilidad de encomiendas.

**Restricción Física del Negocio:** Las rutas interprovinciales en el Altiplano sufren de caídas de red e inestabilidad de conexión. El sistema requiere transacciones de datos altamente consistentes (ACID); por ejemplo, registrar un boleto, bloquear un asiento y actualizar la caja deben ocurrir como una sola operación atómica. Lograr esta consistencia en un entorno de red inestable utilizando sistemas distribuidos (Microservicios) introduce un riesgo altísimo de datos corruptos o transacciones huérfanas.

## 2. Alternativas Consideradas
* **Arquitectura de Microservicios:** Descartada para la Fase 1. La latencia de red interna, la complejidad de mantener la consistencia eventual (patrones Saga/Event Sourcing) y los elevados costos de infraestructura en la nube no se justifican para el volumen transaccional actual de la empresa.
* **Monolito Tradicional (Spaghetti Code):** Descartado debido a la alta deuda técnica que genera, imposibilitando el mantenimiento y escalabilidad a mediano plazo por parte del equipo de Synergy6.

## 3. Decisión Arquitectónica
Se adopta el estilo de **Arquitectura de Monolito Modular**, construido sobre el framework **Spring Boot (Java)**, fundamentado en los principios de Diseño Orientado al Dominio (DDD) y arquitectura limpia.

El sistema se estructura bajo las siguientes directrices:
* **Despliegue Centralizado:** Un único artefacto ejecutable (`.jar`) que contiene todos los dominios del negocio, eliminando la necesidad de un API Gateway complejo. Los clientes web (React) y móviles (Flutter) se comunican directamente con este núcleo.
* **Aislamiento Lógico (Modularidad):** El código se organiza en paquetes estrictamente delimitados por dominio (*Pasajes*, *Encomiendas*, *Seguridad*, *Caja*). Los módulos solo pueden comunicarse entre sí mediante interfaces internas (llamadas en memoria RAM), prohibiendo el acceso directo a la base de datos de otro módulo.
* **Persistencia Centralizada:** Se utilizará un único motor de base de datos relacional (**PostgreSQL**). El orden se mantendrá aislando las tablas por esquemas lógicos correspondientes a cada módulo.

## 4. Consecuencias (Trade-offs)

### ✅ Beneficios Obtenidos
* **Consistencia Absoluta (ACID):** Al usar una base de datos centralizada, si el cobro de un pasaje falla, el motor de PostgreSQL hace un *rollback* automático del asiento y de la caja, garantizando integridad financiera total sin latencia de red.
* **Eficiencia Operativa:** Un solo pipeline de CI/CD, pruebas de integración simplificadas y menor consumo de recursos de CPU/RAM en el servidor (VPS/Cloud).
* **Baja Latencia Interna:** La comunicación entre los módulos de *Encomiendas* y *Liquidación* se ejecuta a nivel de hilos del procesador, reduciendo el tiempo de respuesta al cliente.

### ⚠️ Riesgos y Estrategias de Mitigación
* **Punto Único de Fallo:** Una caída del contenedor principal detiene toda la operación en las terminales.
  * *Mitigación:* Se implementará un balanceador de carga (Load Balancer) frente a múltiples réplicas (instancias) del mismo monolito modular.
* **Degradación a Monolito Tradicional (Acoplamiento):** Los desarrolladores podrían evadir las reglas de modularidad por rapidez, mezclando lógica de diferentes dominios.
  * *Mitigación:* Se configurarán pruebas de arquitectura automatizadas (ej. ArchUnit en Spring Boot) que harán fallar el despliegue si un paquete viola las reglas de dependencia establecidas.
