# 🗣️ 6-Comunicacion — Diagramas de Comunicación de TRANS-SYNC

Este directorio contiene los artefactos de modelado para los **Diagramas de Comunicación** (Collaboration Diagrams) del sistema **TRANS-SYNC**, desarrollados bajo el estándar UML. El propósito de este módulo es complementar los diagramas de secuencia, enfocándose principalmente en la organización estructural y los enlaces lógicos de los objetos que participan en el intercambio de mensajes de negocio.

## 📂 Estructura del Directorio

Tal como se detalla en el árbol de archivos, este directorio está compuesto por los siguientes recursos:

* **📄 `com_rastreo_paquete.puml`:** Script de PlantUML que define la red de interacciones y mensajes lógicos requeridos para llevar a cabo el tracking y rastreo de encomiendas.
* **📄 `Readme.md`:** Documentación guía del directorio actual.

---

## 🔍 Interacciones y Enlaces de Objetos Modelados

A diferencia de los diagramas de secuencia que priorizan el tiempo, este diagrama (`com_rastreo_paquete.puml`) se enfoca en la arquitectura de las conexiones lógicas dentro del ecosistema de **Transportes Veloz Altiplano E.I.R.L.**:

1. **Rastreo de Paquetes:** Describe la arquitectura de mensajería desde que el cliente consulta un estado de envío mediante la app frontal o web, pasando por el API Gateway, hasta la interacción directa con el Microservicio de Encomiendas.
2. **Arquitectura de Red Orientada a Objetos:** Muestra con claridad qué controladores, servicios y repositorios específicos necesitan estar enlazados lógicamente para devolver la trazabilidad de los paquetes en tiempo real.
3. **Bajo Acoplamiento:** Valida que las llamadas de mensajería sigan caminos específicos y respeten las fronteras de las APIs expuestas por cada contenedor.

---

## 🛠️ Instrucciones de Visualización y Edición

1. **Edición:** Abre el archivo `com_rastreo_paquete.puml` en tu editor de código preferido (como VS Code).
2. **Renderizado:** Requiere el uso de la extensión oficial de **PlantUML** en tu entorno para procesar diagramas de colaboración de objetos estándar.
3. **Previsualización:** Presiona la combinación de teclas `Alt + D` para generar de manera automática el esquema gráfico relacional y exportarlo en formato de imagen `.png`, listo para los anexos de la documentación de **Synergy6**.

---

## 🖼️ Vista Previa del Diagrama

![Diagrama de Comunicación](https://img.plantuml.biz/plantuml/png/NPBFJjj04CRlblmENzDBSeZ2dmWX7ohIOAeYGKi8ujBBn3in2-jTTxm-eJuI9nuXByQi4XIeJ-kTRtxpxRTxraMIs3Skpxx41suOhIFhyypnEY86YAqV8emLhg8DMkYUh6z9g47Q8byxndEUGR_lL3tL4dflvi45mLS-MH-jrxjY4CEoAnoifgUdqppxbsTv5crKnhcbMga4mvY7flUseifkNds11NLHc0Ibhq9ZsHl2S2P_UnlLGY-4g-23sxn4xHabvDxQu3TrzCWIC9mxROqy6e0wLDkVJz82ixR5FQyml92WLM-sOchR_uHNcrVJk_31KVV73rC0kiPSqK9kszo4f4okTZCn7dzBI1GuBF3Jry8TeLAYhGEMeX3hQzmiyYofadhBq8QZ0Z_A9IRKsWdlPq-UhT4iTx8z_rZ3unZ44qgzQQCfb8y51kKr5dVBsG1ZNDx-kXxj9xrxB33LK_QioHFwrVjbW3HmSc2FbdmavoYTx4nTw2Dw0m00)
