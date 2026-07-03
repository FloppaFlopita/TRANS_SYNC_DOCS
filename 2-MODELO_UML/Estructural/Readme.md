# 🏗️ Diagramas Estructurales (UML Estático) — TRANS-SYNC

Este directorio contiene los diagramas **estructurales** del sistema **TRANS-SYNC**, desarrollados bajo el estándar UML[cite: 1]. Estos modelos se enfocan en la parte estática del software, especificando la organización lógica, las clases de datos, la jerarquía de paquetes, los componentes lógicos y la disposición física de la infraestructura técnica[cite: 1].

## 📂 Estructura del Directorio

De acuerdo con la organización interna de esta carpeta (ver `image_33759b.png`), los modelos se dividen en los siguientes submódulos lógicos[cite: 1]:

*   **📁 1-Clases:** Contiene el diseño detallado del modelo de dominio, atributos, métodos de negocio y las relaciones lógicas (asociación, agregación, composición y herencia) de cada microservicio[cite: 1].
*   **📁 2-Objetos:** Representa instancias concretas de los elementos del sistema en un momento específico del tiempo, sirviendo para validar la viabilidad del diagrama de clases frente a escenarios reales[cite: 1].
*   **📁 3-Componentes:** Describe la organización, interfaces expuestas y dependencias existentes entre los diferentes módulos o microservicios que integran la plataforma backend[cite: 1].
*   **📁 4-Despliegue:** Mapea la arquitectura física y de red de la infraestructura, especificando cómo se distribuyen los contenedores Docker, los servidores de bases de datos independientes y el API Gateway[cite: 1].
*   **📁 5-Paquetes:** Representa la agrupación lógica y la modularidad del código fuente, organizando el sistema por capas y dominios limpios[cite: 1].
*   **📁 6-Perfil:** Extensiones y personalizaciones del metamodelo UML estándar adaptadas a las necesidades específicas del dominio de transporte y logística[cite: 1].

---

## 🔍 Pilares del Diseño Estructural

Los diagramas estáticos de esta sección aseguran el cumplimiento de las buenas prácticas de ingeniería aplicadas por **Synergy6**[cite: 1]:

*   **Bajo Acoplamiento:** Los diagramas de componentes y paquetes demuestran la independencia de las interfaces lógicas[cite: 1].
*   **Database-per-Service:** El modelo de despliegue valida visualmente que cada base de datos (PostgreSQL) está aislada y vinculada a un único microservicio core[cite: 1].
*   **Principios SOLID:** Las clases están diseñadas respetando la separación estricta de responsabilidades lógicas (SRP) y la inversión de dependencias (DIP)[cite: 1].

---

## 🛠️ Visualización y Modificación

1.  **Código Fuente:** Cada subcarpeta almacena archivos con extensión `.puml` escritos en la sintaxis nativa de PlantUML[cite: 1].
2.  **Compilación:** Utiliza la extensión de **PlantUML** en tu editor de código para procesar los scripts y exportar directamente las imágenes (`.png`) actualizadas hacia los entregables del informe final de análisis de sistemas[cite: 1].