# ⚙️ Diagramas de Comportamiento (UML Dinámico) — TRANS-SYNC

Este directorio contiene los diagramas de **comportamiento** del sistema **TRANS-SYNC**, desarrollados bajo el estándar UML[cite: 1]. Estos modelos se enfocan en la parte dinámica del software, describiendo cómo interactúan los actores con la plataforma, cómo fluyen los procesos de negocio y cómo cambian los estados de los datos a lo largo del tiempo[cite: 1].

## 📂 Estructura del Directorio

De acuerdo con la organización interna de esta carpeta (ver `image_057925.png`), los modelos se dividen en los siguientes submódulos lógicos[cite: 1]:

*   **📁 1-Casos_Uso:** Representa los límites del sistema y las interacciones de los actores principales (Despachador, Conductor, Pasajero, Dueño) con los módulos funcionales de pasajes y encomiendas[cite: 1].
*   **📁 2-Secuencia:** Detalla el intercambio cronológico de mensajes entre los componentes lógicos del sistema frente a escenarios críticos, como la validación de un asiento o la autenticación mediante JWT[cite: 1].
*   **📁 3-Actividades:** Mapea el flujo de trabajo paso a paso de los procesos operativos clave, incluyendo los algoritmos de venta y la lógica del cierre de caja financiero[cite: 1].
*   **📁 4-Estado:** Define el ciclo de vida y las transiciones lógicas de las entidades del negocio (por ejemplo, los estados de una encomienda: *En almacén*, *En ruta*, o *Entregado*)[cite: 1].
*   **📁 5-Tiempos:** Analiza los cambios de estado de los componentes con un enfoque especial en las restricciones y tiempos de respuesta lógicos[cite: 1].
*   **📁 6-Comunicacion:** Describe la interacción organizada entre los objetos del backend, priorizando la estructura de las conexiones por sobre el orden temporal[cite: 1].

---

## 🔍 Procesos de Negocio Modelados

Los diagramas dinámicos de esta sección respaldan de forma directa el flujo operativo de **Transportes Veloz Altiplano E.I.R.L.**[cite: 1]:

*   **Venta de Pasajes:** Evita la sobreventa al centralizar y validar el mapa de los 7 asientos de cada unidad móvil en tiempo real[cite: 1].
*   **Trazabilidad de Encomiendas:** Describe la secuencia lógica desde la recepción del paquete en el counter hasta la firma de entrega final en el destino mediante códigos QR[cite: 1].
*   **Liquidación Diaria:** Flujo de actividades estructurado para consolidar de manera transparente las comisiones e ingresos diarios de los conductores y vendedores[cite: 1].

---

## 🛠️ Visualización y Modificación

1.  **Código Fuente:** Cada subcarpeta contiene archivos con extensión `.puml` escritos en la sintaxis estándar de PlantUML[cite: 1].
2.  **Compilación:** Puedes renderizar estos gráficos utilizando la extensión oficial de **PlantUML** en tu entorno de desarrollo para exportar los diagramas actualizados directamente a los anexos del informe técnico del startup **Synergy6**[cite: 1].