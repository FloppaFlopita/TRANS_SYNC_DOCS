# ⏱️ 5-Tiempos — Diagramas de Tiempos de TRANS-SYNC

Este directorio contiene los artefactos de modelado técnico para los **Diagramas de Tiempos** (Timing Diagrams) del sistema **TRANS-SYNC**, desarrollados bajo el estándar UML. El propósito de este módulo es representar de forma gráfica los cambios de estado de los componentes y las restricciones de tiempo lógicas ante eventos concurrentes y críticos del sistema.

## 📂 Estructura del Directorio

Tal como se detalla en el árbol de archivos, este directorio está compuesto por los siguientes recursos:

* **📄 `tiempos_reserva.puml`:** Script de PlantUML que modela las variaciones de estado de los objetos a lo largo del tiempo durante un proceso lineal de reserva rápida.
* **📄 `Readme.md`:** Documentación guía del directorio actual.

---

## 🔍 Restricciones y Estados Temporales Modelados

El diagrama contenido en este módulo especifica con alta precisión el comportamiento dinámico y las restricciones de respuesta para **Transportes Veloz Altiplano E.I.R.L.**:

### Objetivos del Modelado de Tiempos (`tiempos_reserva.puml`):
1.  **Control de Bloqueos Temporales:** Define la duración exacta del estado *Asiento Bloqueado* desde que el counter inicia la selección en Juliaca o Cusco, otorgando una ventana de tiempo máxima (ej. 5 minutos) antes de liberar el asiento automáticamente para evitar el desabastecimiento artificial.
2.  **Sincronización de Componentes Internos:** Analiza las transiciones de los hilos de ejecución en el backend y los tiempos de respuesta permitidos para que el módulo de Pasajes actualice la base de datos centralizada compartida.
3.  **Ciclo Crítico:** Mapea de forma temporal la secuencia de estados del asiento: `Libre` ➡️ `Bloqueo Temporal (Pendiente de Pago)` ➡️ `Vendido / Confirmado` o su retorno a `Libre` por tiempo de espera agotado (Timeout).

---

## 🛠️ Instrucciones de Visualización y Edición

1.  **Edición:** Abre el archivo `tiempos_reserva.puml` en tu editor de código preferido (como VS Code).
2.  **Renderizado:** Asegúrate de contar con la extensión oficial de **PlantUML** instalada en tu entorno de desarrollo para procesar la sintaxis de diagramas de tiempo (`@robust` o `@concise`).
3.  **Previsualización:** Presiona la combinación de teclas `Alt + D` para procesar el código en tiempo real y exportar el diagrama estructurado en formato de imagen `.png`, dejándolo listo para anexarlo a la sección de análisis avanzado de tu informe de **Synergy6**.

---

## 🖼️ Vista Previa del Diagrama

![Diagrama de Tiempos de Reserva](https://img.plantuml.biz/plantuml/png/XP7HQi8m58Rl0ts7Cw-s2w5rUg5NXhHAn4PfesExALaDcf4sfKdtLdkAlTYoJXmEP1U1m7--_-CaS-j4wxfA1-ZEdMGbeT52rG5ooca9iHB7LbG23XAuabLZx0psIhn9M7LQYLB044XdImFtgQhLkwZXPOo7qUZH1xcoJdeuDRNHdnzEbUOXG05gpMjd7GmIBpyOE8C341Qgdtk0IbENoaeOuARnTWt4r8UkTARjvqJJV3VDmm2T4L0M4bRm94ifm-jYjLjJJ720_EXtHZOi8Hp7c-A9BcWFHvE_TBRZlmJFCCjJocd2FBNSviLusNFJQ-iMPpZ6tamO9RZ0ptXFC_f_JHJUyFjiDBwz6TdbP7EfNr1MnCc5FAdZIVlZ89g0Cp0DOGRS_w61w2eD-zXxBlceDql_p9N-0W00)
