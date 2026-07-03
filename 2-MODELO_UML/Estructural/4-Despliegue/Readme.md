# 🚀 4-Despliegue — Diagrama de Despliegue de TRANS-SYNC

Este directorio contiene los artefactos de modelado técnico para el **Diagrama de Despliegue** del sistema **TRANS-SYNC**, desarrollado bajo el estándar UML. El objetivo de este módulo es mapear la arquitectura física y de red de la infraestructura, especificando cómo se distribuyen los nodos de hardware, el entorno de ejecución del monolito y la base de datos del proyecto.

## 📂 Estructura del Directorio

Tal como se detalla en el árbol de archivos actual, este directorio está compuesto por los siguientes recursos:

* **📄 `diagrama_despliegue.puml`:** Script de PlantUML que define la distribución física de los servidores, el contenedor principal de la aplicación, las redes internas y el almacenamiento de la base de datos.
* **📄 `Readme.md`:** Documentación guía del directorio actual.

---

## 🔍 Distribución e Infraestructura Física Modelada

El archivo `diagrama_despliegue.puml` valida e ilustra de manera exacta la infraestructura de producción planificada por **Synergy6** para operar en las sedes de **Transportes Veloz Altiplano E.I.R.L.**:

1. **Servidor en la Nube (Cloud Infrastructure):** Modelado del servidor virtual centralizado (VPS/AWS Node) que aloja el sistema.
2. **Entorno de Ejecución Central (Monolito Modular):** Nodo lógico que aloja el contenedor de la aplicación principal (ej. Spring Boot), donde conviven todos los módulos de negocio altamente cohesivos.
3. **Servidor Web / Proxy Inverso:** Configuración del servidor (ej. Nginx) encargado de recibir las solicitudes de red HTTPS/JSON de los clientes y enrutarlas directamente a la aplicación central por la red privada.
4. **Persistencia de Datos (Base de Datos Centralizada):** Demostración visual del nodo de almacenamiento relacional (PostgreSQL) compartido por todos los módulos del sistema, garantizando la integridad transaccional (ACID).
5. **Nodos de Dispositivos Cliente (Client Nodes):** Computadoras físicas en las terminales de counter de Juliaca y Cusco para la aplicación web (React) y teléfonos móviles de los conductores para la aplicación nativa (Flutter).

---

## 🛠️ Instrucciones de Visualización y Edición

1. **Edición:** Abre el archivo `diagrama_despliegue.puml` en tu editor de código preferido (como VS Code).
2. **Renderizado:** Asegúrate de contar con la extensión oficial de **PlantUML** instalada en tu entorno de desarrollo para procesar la sintaxis de infraestructura estándar de UML (`node`, `artifact`, `database`).
3. **Previsualización:** Presiona la combinación de teclas `Alt + D` para procesar el código en tiempo real y exportar el diagrama estructurado en formato de imagen `.png`, quedando listo para anexarlo a tu documentación técnica y presentación académica final.

---

## 🖼️ Vista Previa del Diagrama

![Diagrama de Despliegue](https://img.plantuml.biz/plantuml/png/ZLFDRjD04BvRyZiCuK1wI8Cgojy1rN6AA6fJ4uT6I4Xex9sORJUxxkuwhOHu94vzXBmOixP3L24aVB1aZx_VMPyuZzOtQnL7J_ntMXFK2gME8tSZTOqMrw2D8FWHHy3N1CkRoff6YzGeO-4f7T7hrVD-QAmWsmzUl3e-VlacZdx6KHnvwHN1L6B5X0ZCDoLNAqbLGp22nJoPvQFyooo5OM9l6-cfz8r5k33QgEqlBqiy23ojbS5KkjeuwUN6mCNsOIFLLprCjB162XY3lCmF1e0EreP7E-USKgwmz318wdeFUwyQxybs0Aphtd0db9frtNWKXgsCOK5sBJMgOF-Aj4U6BwKMvixnz5pgvhwZgSk_HMUueIemmPAAe6kDzgG5v5dIeUweU2IUazt80E27XBigiPJR1ytOq-j3kCfo5asMEPocHns1Om3PdNJ9tercco7m7pIa_CPoXdtbJ9ZNLkgAzsSy75wZtTN7vKjl_kbgWexQNQ8thlSL7Csd_G94yUsnAO4UYu0QFCB2PorNR564IZFZV6Kf_tJUaHIYD_0CKWvqB_dc0bGniEGpn3towbIRFrYB8zuZZ4RlTesyXJF-nchoCFomMBJDVSmlPtoakFJ__7Al7seKjDS318LGz85421H7k_9Qza8myvm4P5PkE2KC5sasFii2-tIIjkmdV1ZuD_mD)
