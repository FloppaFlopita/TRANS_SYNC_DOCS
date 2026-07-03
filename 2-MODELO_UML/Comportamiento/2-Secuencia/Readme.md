# ⏳ 2-Secuencia — Diagramas de Secuencia de TRANS-SYNC

Este directorio contiene los artefactos de modelado técnico para los **Diagramas de Secuencia** del sistema **TRANS-SYNC**, desarrollados bajo el estándar UML. El propósito de este módulo es detallar el intercambio cronológico de mensajes e interacciones entre los diferentes objetos del backend y las capas de software ante flujos operacionales críticos.

## 📂 Estructura del Directorio

Tal como se detalla en el árbol de archivos actual (ver `image_0575c2.png`), este directorio está compuesto por los siguientes recursos:

* **📄 `seq_vender_pasaje.puml`:** Código fuente PlantUML enfocado específicamente en la lógica temporal y cronológica de la reserva de asientos, validación de disponibilidad en tiempo real y cálculo de tarifas para la venta de pasajes.
* **📄 `Readme.md`:** Documentación guía del directorio actual.

---

## 🔍 Interacciones y Flujos Técnicos Modelados

El diagrama contenido en este módulo especifica el comportamiento paso a paso del software de **Transportes Veloz Altiplano E.I.R.L.**:

1. **Validación Perimetral:** Detalla el paso de los mensajes a través del API Gateway y la verificación del token de seguridad para asegurar que el usuario tenga los permisos correspondientes.
2. **Aislamiento de Capas:** Describe de forma exacta el recorrido de la petición en el backend: `Controller` ➡️ `Service` (Lógica de Negocio) ➡️ `Repository` (Acceso a Datos) ➡️ `Base de Datos Privada`.
3. **Control de Concurrencia:** Modela las llamadas lógicas necesarias para asegurar que el mapa de 7 asientos de cada unidad móvil se mantenga sincronizado en tiempo real, erradicando los problemas de sobreventa entre las sedes de Juliaca y Cusco.

---

## 🛠️ Instrucciones de Visualización y Edición

1. **Edición:** Abre el archivo `seq_vender_pasaje.puml` utilizando tu editor de código preferido (como VS Code).
2. **Renderizado:** Asegúrate de contar con la extensión oficial de **PlantUML** configurada en tu entorno de desarrollo para procesar diagramas secuenciales.
3. **Previsualización:** Presiona la combinación de teclas `Alt + D` para generar de manera automática el esquema gráfico dinámico y exportarlo en formato `.png`, dejándolo listo para los informes de desarrollo de **Synergy6**.

---

## 🖼️ Vista Previa del Diagrama

![Diagrama de Secuencia TRANS-SYNC](https://img.plantuml.biz/plantuml/png/XLNBRjDG4DrRyZ-CoYQHG2s8Kl02KH8U1K8hKi4c4fhuJjrfh-yru-j0GNmCInQi-8Jy67FZ9CsZ5LdaDNUEpvnpndvM1vJGb3PDi0dUDUMO94tgItOL2fPGuhS1rJKMDEJl1FVtzrQh-XuuvmfTW1zf0lfwZlbb8RvnfkUj5xX33-ZnsTwywCMGp0iF3_Rt7pr9avzfaYQ1WoNeCnQAYs08XfGtv7B633wIqpPe79nWZHS4dKFvqd2WF3I2CF3Es-aVPOBTY8LvKFoTFjKLvkTel8nSfwUK0abt1x1M-6KfJLQ7s3ciAlX4OsruALuRd6axlj9uu-HW-jSqriDXewVYjNEU_dMnaMqG3yDAs1MpCOJ3LGjJUlDPXJw_1QiThrQG8Sc4SxhkgjhIBOtlMFKmImg7ZM7LOFe7OGi8snfZb6f52BZtD4u9cRPOodFs3a6QW7UratL4VtVaT2AX6g7__WYk8FVkZ4NjccWPPyBp10ErQgL9X5FKnT0AVN8yF8LTh7XtrX8dVKsevcPmwY_9mPjFfzqLe6kzqiHv_KEuE0_WpvQL35vOE6ibv-XmJbN0aRC85KMXL16eTBoQ2ZN2e8bOIqhhz3wYrHDopKNvVV0sWvKiTM_gdxkZ44TkukTPQFaup4PkCajmQs_7OF3rvfHBVrlm1U0M_eAYuRhoZiSSVvgHmYzigg4pcFxw1WVT_q2TaDHS1vRMFz2Hd_UXfzy5xSsApvipwFcoSOlGAndHNLJLIpAimIImLjVOQEGGokdlu8tIiYgClNN4PIxNHSn0g52MWd8q2v_luGLsIXy3kRh8sx5PvdmT_eRhlMfGegZM5vigRFHkYVY1jE9yl6FHXUvwAqXdujdi7h_jnXMxZTQ63EjHF1vVABBUCMtyACYHw9HRS1knQJEvtEG7U_UX9wI73NJwCNRAqyAu1NqpF7v_4y5stMRBgqYhjuWC1Wr5BwB_bVXnz5ftv9qQvEFJ087rVovPre7dDuHdkWRwiFa7)
