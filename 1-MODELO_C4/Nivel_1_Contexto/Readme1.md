# 🏢 Nivel 1: Diagrama de Contexto — TRANS-SYNC

Este directorio contiene el modelado arquitectónico de **Nivel 1 (Contexto)** para el sistema **TRANS-SYNC**[cite: 1]. Este nivel establece el alcance global del proyecto, definiendo cómo la plataforma interactúa con los usuarios externos y los roles clave del negocio de transporte interprovincial y encomiendas rápidas[cite: 1].

## 📂 Estructura del Directorio

Tal como se observa en el árbol de archivos (ver `image_298ff6.png`), este módulo contiene los siguientes componentes esenciales[cite: 1]:

*   **📄 `c4_nivel1_contexto.puml`:** Archivo fuente en lenguaje PlantUML que contiene el código y la definición de los actores, el sistema central y las relaciones/flujos entre ellos utilizando la librería estándar C4[cite: 1].
*   **📄 `Readme.md`:** Documentación guía del directorio actual[cite: 1].

---

## 🔍 Descripción del Diagrama de Contexto

El diagrama representa al sistema **TRANS-SYNC** en el centro del ecosistema operativo y describe las interacciones con los principales **Stakeholders** de la empresa[cite: 1]:

1.  **👤 Despachador (Counter):** Registra la venta rápida de pasajes y la recepción de encomiendas desde las terminales terrestres (Juliaca y Cusco)[cite: 1].
2.  **👤 Conductor en Ruta:** Reporta el inicio/fin de ruta, incidentes en la carretera y la entrega de encomiendas desde la unidad móvil[cite: 1].
3.  **👤 Dueño / Gerente:** Supervisa la rentabilidad, visualiza los reportes de ventas y el desempeño general del negocio[cite: 1].
4.  **👤 Pasajero / Cliente:** Compra boletos de viaje y consulta el estado de rastreo de sus paquetes[cite: 1].

### Flujos Principales Modelados:
*   Emisión de tickets físicos y generación de códigos de rastreo logístico[cite: 1].
*   Actualización de ubicación y estados del viaje en tiempo real[cite: 1].
*   Consolidación y envío de reportes de desempeño y ventas hacia la administración[cite: 1].

---

## 🛠️ ¿Cómo visualizar o modificar el diagrama?

1.  **Modificación:**
    *   Abre el archivo `c4_nivel1_contexto.puml` en tu editor de código preferido (como VS Code).
    *   Asegúrate de tener instalada la extensión de **PlantUML** para procesar la sintaxis de la librería `C4_Context.puml`[cite: 1].
2.  **Previsualización:**
    *   Presiona `Alt + D` (en VS Code) para renderizar el diagrama en tiempo real.
    *   Puedes exportar el resultado final directamente en formato `.png` o `.svg` para adjuntarlo a tus informes técnicos de la universidad[cite: 1].