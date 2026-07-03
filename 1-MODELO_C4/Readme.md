# 🗺️ 1-MODELO_C4 — Diseño Arquitectónico de TRANS-SYNC

Este directorio contiene la documentación gráfica y el modelado conceptual del sistema **TRANS-SYNC** siguiendo la metodología del **Modelo C4**[cite: 1]. El objetivo es estructurar la arquitectura en diferentes niveles de abstracción para facilitar la comprensión técnica tanto de los desarrolladores como de los stakeholders del negocio[cite: 1].

## 📂 Estructura del Directorio

Tal como se muestra en la estructura de archivos de la carpeta (ver `image_298bf3.png`), este módulo se divide en tres niveles fundamentales[cite: 1]:

*   **📁 Nivel_1_Contexto:** Define el alcance global del sistema, mostrando cómo TRANS-SYNC interactúa con los usuarios (Despachadores, Conductores, Dueño) y delimitando las fronteras de la aplicación[cite: 1].
*   **📁 Nivel_2_Contexto:** (Contenedores) Descompone el sistema en aplicaciones web, móviles y microservicios independientes, detallando los flujos de comunicación y las tecnologías de persistencia de datos asociadas[cite: 1].
*   **📁 Nivel_3_Contexto:** (Componentes) Entra al detalle interno de cada microservicio, mostrando la organización en capas (Controladores, Servicios, Repositorios) y sus interacciones internas[cite: 1].

---

## 🔍 Resumen de los Niveles Implementados

### 🏢 Nivel 1: Diagrama de Contexto
*   **Enfoque:** Mostrar el ecosistema del sistema desde una perspectiva de alto nivel[cite: 1].
*   **Actores Clave:** Despachador (Counter), Conductor en Ruta, Dueño/Gerente y el Pasajero/Cliente[cite: 1].
*   **Flujo:** Registro de pasajes/encomiendas en sucursales e informes en ruta hacia la plataforma central[cite: 1].

### 📦 Nivel 2: Diagrama de Contenedores
*   **Enfoque:** Identificar las aplicaciones tecnológicas y la separación de responsabilidades en el ecosistema[cite: 1].
*   **Componentes de Red:** Frontend Web (React), Mobile App (Flutter), un API Gateway unificado (Ocelot/Nginx) y múltiples microservicios[cite: 1].
*   **Estrategia de Datos:** Patrón de base de datos independiente por servicio para mitigar el acoplamiento y asegurar la tolerancia a fallos[cite: 1].

### ⚙️ Nivel 3: Diagrama de Componentes
*   **Enfoque:** Arquitectura interna de los microservicios core[cite: 1].
*   **Servicios Modelados:** Pasajes, Encomiendas, Autenticación (Auth), Usuarios y Liquidación[cite: 1].
*   **Patrón Estructural:** Separación estricta usando interfaces, DTOs y encapsulamiento bajo principios SOLID[cite: 1].

---

## 🛠️ Herramientas de Visualización

Todos los diagramas alojados en los subdirectorios han sido desarrollados utilizando la librería estándar **C4-PlantUML**[cite: 1]. Los archivos de origen cuentan con la extensión `.puml` para que puedan ser modificados o regenerados fácilmente utilizando la extensión de PlantUML en tu entorno de desarrollo o mediante su servidor oficial[cite: 1].