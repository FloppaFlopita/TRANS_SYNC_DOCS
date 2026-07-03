# 📦 5-Paquetes — Diagrama de Paquetes de TRANS-SYNC

Este directorio contiene los artefactos de modelado técnico para el **Diagrama de Paquetes** del sistema **TRANS-SYNC**, desarrollado bajo el estándar UML[cite: 1]. El objetivo de este módulo es representar de forma gráfica la organización lógica, la modularidad y la jerarquía del código fuente del proyecto, agrupando las clases en subsistemas lógicos y delimitando sus dependencias mutuas[cite: 1].

## 📂 Estructura del Directorio

Tal como se detalla en el árbol de archivos actual (ver `image_339347.png`), este directorio está compuesto por los siguientes recursos[cite: 1]:

* **📄 `diagrama_paquetes.puml`:** Script de PlantUML que define la agrupación por paquetes del software, mostrando la separación por capas y las relaciones de dependencia entre los distintos módulos[cite: 1].
* **📄 `Readme.md`:** Documentación guía del directorio actual[cite: 1].

---

## 🔍 Organización y Modularidad Modelada

El archivo `diagrama_paquetes.puml` ilustra visualmente la arquitectura de software limpia aplicada por **Synergy6** para estructurar el backend del ecosistema[cite: 1]:

1. **Abstracción por Dominios:** Agrupa de forma estricta las funcionalidades lógicas del negocio de **Transportes Veloz Altiplano E.I.R.L.** en paquetes independientes (Pasajes, Encomiendas, Autenticación, Usuarios y Liquidación)[cite: 1].
2. **Separación por Capas (Layered Structure):** Dentro de cada paquete de microservicio, se detalla la subdivisión interna en carpetas lógicas para garantizar el orden del código fuente[cite: 1]:
    * `controller`: Capa que expone los endpoints REST RESTful de la aplicación[cite: 1].
    * `service`: Contenedor de las reglas de negocio y algoritmos de orquestación[cite: 1].
    * `repository`: Capa encargada del acceso y persistencia de datos[cite: 1].
    * `model` / `entity`: Definición de los objetos y tablas de datos lógicos[cite: 1].
    * `dto`: Objetos de transferencia de datos para optimizar los mensajes HTTPS/JSON[cite: 1].
3. **Control de Dependencias:** Valida de manera gráfica el acoplamiento directo entre capas, asegurando que las dependencias fluyan de manera unidireccional y respeten los principios de diseño de software[cite: 1].

---

## 🛠️ Instrucciones de Visualización y Edición

1. **Edición:** Abre el archivo `diagrama_paquetes.puml` en tu editor de código preferido (como VS Code)[cite: 1].
2. **Renderizado:** Asegúrate de contar con la extensión oficial de **PlantUML** instalada en tu entorno de desarrollo para procesar la sintaxis de agrupación estándar de UML (`package`, `folder`)[cite: 1].
3. **Previsualización:** Presiona la combinación de teclas `Alt + D` para procesar el código en tiempo real y exportar el diagrama estructurado en formato de imagen `.png`, quedando listo para integrarlo de forma directa a la documentación técnica de tu informe universitario[cite: 1].

https://img.plantuml.biz/plantuml/png/ZPJDRXf13CVlIBo3ImybXzAgXwhAeKe2790QDI9HJrpCh9TCCpkUp7YZeee7wY6dFW8l5ky77orGTIu8-sVxFnvxBv9WbB9mtSuhkQU283Yqljj93zO7Z5X0GFE02xgLfIF8sMKKzzrpTIyYbpuRikC8h_FwT3lTZbZHa975XO886S4DFfOabE0jNAz_PwLZDINyhfR-PNmihP2HCY9SisUtVXPhyAnArOg0Ng21uM8W4NrAIsy6eOdlQU7t-QSyXvyL3tgsCOQzH7QEebBqCV_GKD0Uup2bZOxXbjq1deLWpY9SdCFuHs1Fe35mUJD9CzyV-oomzP9WEhwzEslYLWSg4iKdQ-Ye18sccACXc3GwRXlukCZMEIc2Eo5oIejAe7RSquADvPbVWdFw2fcQwseUqocbaG8dAnoN_oTskkLFoD6cfjA9biQPTmXNcAWIDqBX14FIbgCxfQRWZDnH8Lj44rXHiNk-NS-ks97mCS-q5DpPLqSIPy8didxJcZWb7USaexkl_q2IpakYFvZLzgxrTT_0Y0BvZBonsgEg7Rg7crNfVr5RxiZSwszHrTFP1zsLzI_Vl2bW-rTdRpVhC1XyXdReu1nwK2Ri7G1wmzePoTWvlIF_j7wkC5tnDhIYTXEnbsaVQ5wWTeR8XWw0JPq20pNvztB-dO5YiacenYwqCVfzUW40
