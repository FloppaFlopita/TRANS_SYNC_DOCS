# 📊 2-MODELO_UML — Modelado del Sistema TRANS-SYNC

Este directorio contiene toda la especificación técnica de modelado visual para el proyecto **TRANS-SYNC**, estructurada bajo el estándar **UML** (Unified Modeling Language)[cite: 1]. El objetivo de este módulo es definir con precisión tanto la estructura interna del software como el comportamiento dinámico de los procesos de negocio (pasajes y encomiendas)[cite: 1].

## 📂 Estructura del Directorio

Tal como se observa en el árbol de archivos (ver `image_33715c.png`), la documentación UML está organizada en dos grandes bloques de diseño:

### ⚙️ 1. Comportamiento (Diagramas Dinámicos)
Muestra cómo fluye la información y cómo interactúan los objetos del sistema a lo largo del tiempo:
*   **📁 1-Casos_Uso:** Define las interacciones entre los actores (despachador, conductor, dueño) y los límites lógicos del sistema[cite: 1].
*   **📁 2-Secuencia:** Detalla la comunicación cronológica paso a paso entre los componentes frente a un evento específico (ej. validación de pasajes o tracking de carga)[cite: 1].
*   **📁 3-Actividades:** Representa los flujos de trabajo operativos y algorítmicos (como el proceso de cierre de caja)[cite: 1].
*   **📁 4-Estado:** Describe el ciclo de vida de las entidades críticas (ej. una encomienda: *En Almacén*, *En Ruta*, *Entregado*)[cite: 1].
*   **📁 5-Tiempos:** Analiza las restricciones temporales y cambios de estado basados en eventos del sistema[cite: 1].
*   **📁 6-Comunicacion:** Se enfoca en la organización de los objetos que participan en el intercambio de mensajes lógicos[cite: 1].

### 🏗️ 2. Estructural (Diagramas Estáticos)
Define la organización lógica y física de los componentes de código del software:
*   **📁 1-Clases:** Contiene la estructura detallada del modelo de datos, atributos, métodos y sus relaciones lógicas[cite: 1].
*   **📁 2-Objetos:** Instancias concretas del diagrama de clases en momentos específicos del tiempo[cite: 1].
*   **📁 3-Componentes:** Muestra la organización y las dependencias entre los módulos lógicos o microservicios de software[cite: 1].
*   **📁 4-Despliegue:** Mapea la distribución física de la infraestructura, servidores y contenedores de base de datos[cite: 1].
*   **📁 5-Paquetes:** Agrupación lógica de las capas y submódulos que componen el código fuente[cite: 1].
*   **📁 6-Perfil:** Extensiones y personalizaciones del metamodelo UML adaptadas al dominio del transporte[cite: 1].

---

## 🛠️ Visualización y Modificación

*   **Formato de archivos:** Los diagramas están construidos utilizando scripts de **PlantUML** (`.puml`) para asegurar un mantenimiento ágil a través de código limpio[cite: 1].
*   **Edición:** Puedes abrir cualquier subcarpeta, modificar el archivo fuente en tu editor favorito y compilar utilizando la extensión oficial de PlantUML para renderizar y actualizar las imágenes de los anexos del informe[cite: 1].