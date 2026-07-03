# 💎 2-Objetos — Diagramas de Objetos de TRANS-SYNC

Este directorio contiene los artefactos de modelado técnico para los **Diagramas de Objetos** del sistema **TRANS-SYNC**, desarrollados bajo el estándar UML. El propósito de este módulo es representar instancias concretas y reales de los elementos del sistema en un momento específico del tiempo, sirviendo como una herramienta de validación para el diagrama de clases frente a escenarios prácticos del negocio.

## 📂 Estructura del Directorio

Tal como se detalla en el árbol de archivos actual (ver `image_338f45.png`), este directorio está compuesto por los siguientes recursos:

* **📄 `objetos_boleta_real.puml`:** Script de PlantUML que define un caso de prueba real mapeando la instanciación de un boleto físico/digital de viaje emitido con datos concretos del negocio.
* **📄 `Readme.md`:** Documentación guía del directorio actual.

---

## 🔍 Caso de Instanciación Práctica Modelado

El archivo `objetos_boleta_real.puml` aterriza la abstracción del diagrama de clases a un ejemplo del día a día en **Transportes Veloz Altiplano E.I.R.L.**:

1. **Datos del Cliente/Pasajero:** Muestra un objeto concreto con atributos reales (Nombre, DNI, Teléfono).
2. **Asignación Física de Asiento:** Instancia de forma exacta la ocupación de uno de los 7 asientos disponibles en una unidad vehicular con placa y chofer asignados en la ruta Juliaca - Cusco.
3. **Comprobante de Pago (Boleta):** Detalla los valores reales guardados en memoria al procesar la venta: número de boleta, fecha, hora exacta, subtotal y el estado de la transacción.

Este modelado ayuda a verificar que las relaciones de multiplicidad y composición definidas en la arquitectura estructural funcionen correctamente al momento de procesar un flujo de venta real en las terminales.

---

## 🛠️ Instrucciones de Visualización y Edición

1. **Edición:** Abre el archivo `objetos_boleta_real.puml` en tu editor de código preferido (como VS Code).
2. **Renderizado:** Asegúrate de contar con la extensión oficial de **PlantUML** configurada en tu entorno de desarrollo para procesar la sintaxis de instanciación de objetos.
3. **Previsualización:** Presiona la combinación de teclas `Alt + D` para procesar el código en tiempo real y exportar el esquema gráfico en formato de imagen `.png`, quedando listo para anexarlo a tu informe final de **Synergy6**.

---

## 🖼️ Vista Previa del Diagrama

![Diagrama de Objetos](https://img.plantuml.biz/plantuml/png/NL9BRjim5DmBq1rUrKsxK27v5zX0WSXEKI15ui1E3RGRuvcaRJeIgVAJHOiUgQVenVf8Abs4Asg6d9atuhLrQ9plsZnxuywY4z2tA5MUsIUfUZJOWJvS17FmAy-0rXBPqybeh_XAjzh0soC_7evN0waD5sOWnd7bsUyyopCdNIlWHkA9916uW3N9EcqNi5NOsxDs0VGAOIUKGoZXSTFSRyljj_iLl6lC3oyTnV06uKuhtVxzuoJ3zq5x25XSFAe7OSHFMC1Nwz58NG1QyDQaz4Qty16AXsRRt7xQh8k0SIK3TbNLe_5aEekOqjt121lmMz8iXXbUV8ntkA-hATbiQ1iz0fPCj94deTBTLYB3P2Eiaqe7UEKjqn6awkKHbsW5uTFgGrMzSZhebZhQDsEoMiPzD4jmifCy4K7vyKivdrTrci5tmkZ6IcepaEC07WKxuqxY9HWMeseqAwjPMS-XhXRZ2fgxU9MY8jUfgS_DpVhr_9rKyXdLVbTJh9quI-RR5Env-4ZHw2Kn33BV9qr9zKPnXZqooP4J4LyDfeXspNnFjg7roM0OVbnPleoxW0AOxdeJ6XqmOcFpWUk5SK899Y0SY33H_oE58-HrKiWndiYpQw4uFVr_)
