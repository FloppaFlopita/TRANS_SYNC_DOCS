# 🗂️ 1-Clases — Diagrama de Clases Estructural de TRANS-SYNC

Este directorio almacena el modelado lógico estático de las entidades que componen la plataforma de software **TRANS-SYNC**, desarrollado bajo el estándar de diagramas de clases de UML. En esta sección se mapean formalmente los modelos de datos, sus atributos, los métodos operativos y las relaciones lógicas del sistema.

## 📂 Estructura del Directorio

Tal como se observa en el árbol de archivos actual (ver `image_338c3f.png`), el directorio cuenta con los siguientes elementos:

*   **📄 `diagrama_clases.puml`:** Código fuente escrito en lenguaje PlantUML que define las clases lógicas, interfaces y las relaciones de asociación, composición y herencia de los microservicios.
*   **📄 `Readme.md`:** Documentación e instrucciones guía del directorio.

---

## 🔍 Descripción del Modelo de Dominio

El archivo `diagrama_clases.puml` consolida de manera organizada la arquitectura de datos del proyecto para **Transportes Veloz Altiplano E.I.R.L.**:

1.  **Módulo de Viajes y Rutas:** Define las clases que controlan los horarios de salida entre las sedes de Juliaca y Cusco, y el mapeo exacto de los 7 asientos por unidad móvil para erradicar por completo los problemas de sobreventa.
2.  **Módulo de Logística (Encomiendas):** Clases dedicadas a estructurar los registros de carga, peso, remitentes, destinatarios y los estados para el rastreo en ruta mediante códigos QR.
3.  **Módulo de Seguridad y Usuarios:** Modela las entidades de empleados, conductores, asignación de permisos según el rol y el manejo de credenciales para la autenticación perimetral JWT.
4.  **Módulo de Liquidación y Caja:** Estructura las clases encargadas de auditar el dinero que ingresa diariamente en cada terminal de counter.

---

## 🛠️ Instrucciones de Visualización y Edición

1.  **Modificación:** Abre el archivo `diagrama_clases.puml` utilizando tu editor de código favorito (como VS Code).
2.  **Renderizado:** Asegúrate de tener activa la extensión oficial de **PlantUML** en tu entorno para procesar los scripts estructurales.
3.  **Previsualización:** Presiona las teclas `Alt + D` para compilar el código en tiempo real y exportar el gráfico en formato `.png` o `.svg`, listo para acoplarlo como anexo al informe final de **Synergy6**.

---

## 🖼️ Vista Previa del Diagrama

![Diagrama de Clases Estructural](https://img.plantuml.biz/plantuml/png/XLPDRzD04Br7odyOp84M53vEY4WWN3k20asBao9nGbDxwWwiTyFkkWSGFuaJFw5_ZB4TfqwoXUGGP-RjxjitRoPvxJnQNrTgFBhdhwWYM2baFHwvRwnNQB62NA5piVUMBsfFnxdH2_v1y7Gy6eyyUqMGCfQ2H2W84a6JWmaiitY-c2m-pnCuYEttcZtblhO89qORTVFRSuw7pHuhpBzXIH2TtFmfQcMcSEvgj6mS41mNf3qNM4Hm__95yuQVun78gwNLG_jWyve05-lm53uONGvJXUOfBEGkss5jgWjBBfJ25Id5XGacSqj2C6TK-zb7WAANRkvf3mwdS6IC8jHR05445Vz0cw8tha5T6ouwoAz6dEQ1T5r1PjJmakdvR7uw-3fRdCN9spWzpMw3oUayFK-MVMYpNw_Pv5MxwnGYpwG9daNZqQzmHSxGuLToTnJX4rrnBhZTAlJn_JA8oN8C2efoU5FlAHnhJoLPU0dFXmWInnRc12MhkHBYteIqjxGoLhmzQ-5tADlHpsgFkzIRs3vjOxaa7U9T22tM0IOJ419yYKVI5bD8JNsXQCXJsidLIZ0fkvNHVC6gkVwUONOu7qdAxmdUHVTvYu78cjYjrLehEqHSKdw5drYAB2JHqv8hsYfOQm1hqd3_zEbvsqT15On7TOQb52Ca0rNisNRyjulLvL7N2eFvZJ1j6QDd4JoSJ21w6FKQYRz5vDRYKOVS-BL1hy7jQe6Yur8BIS2xks6cSzCuhy2xEk8MiLsYt1HScgMLBKMVe94qPuqOKgcWZf9FMw-XxoPSq8kvvLNE9cZL5JdpljmlWcGioQ84ROcXTDTvSltsiuKDIoITGLOQplFtcZn-p89rt4oyTMFgcgvDz_oFwJSuSYZeRFub_d0I9xFvLYmxNyR3m3ARlP7HkBFne4Oo2OSdz1EnTy03o4W6bkWflsnI64jGTLvmS3185Im2Ucmme12EKaWQD2fu0k_EOlcrwqTlOxp7Zr_jsFHQo10SI7t5SrT2nnv6uJK3xhBEKibEpld_KldScB_hYwBEvSYaVV3Tgl7ejUmi_md-0W00)
