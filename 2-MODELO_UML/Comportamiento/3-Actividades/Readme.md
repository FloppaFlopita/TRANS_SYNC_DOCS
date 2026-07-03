# 🔄 3-Actividades — Diagramas de Actividades de TRANS-SYNC

Este directorio contiene los artefactos de modelado lógico para los **Diagramas de Actividades** del sistema **TRANS-SYNC**, desarrollados bajo el estándar UML. El propósito de este módulo es representar de forma gráfica los flujos de trabajo operativos, algoritmos de negocio y secuencias de pasos que ejecutan los usuarios o los servicios del sistema para cumplir los procesos core de la empresa.

## 📂 Estructura del Directorio

Tal como se detalla en el árbol de archivos (ver `image_338408.png`), este directorio está compuesto por los siguientes recursos:

*   **📄 `act_cierre_caja.puml`:** Script de PlantUML que define el diagrama de actividades para el proceso financiero de cierre de caja, modelando la recopilación de ingresos, validaciones y auditoría automatizada.
*   **📄 `flujo_registrar_venta.puml`:** Código fuente PlantUML que detalla las etapas algorítmicas secuenciales y de decisión lógica al registrar una nueva venta o reserva de pasaje interprovincial.
*   **📄 `Readme.md`:** Documentación guía del directorio actual.

---

## 🔍 Procesos Operativos y Algorítmicos Modelados

Los diagramas contenidos en este módulo especifican el comportamiento de los flujos de trabajo de **Transportes Veloz Altiplano E.I.R.L.**:

1.  **Registro de Venta (`flujo_registrar_venta.puml`):** Modela visualmente las decisiones del sistema desde que se seleccionan los asientos, se consulta la disponibilidad en tiempo real entre las sedes (Juliaca y Cusco) para evitar duplicados, se procesa el cobro y se emite el comprobante físico o electrónico de viaje.
2.  **Cierre de Caja (`act_cierre_caja.puml`):** Detalla las actividades y bifurcaciones condicionales que realiza el contador digital del sistema: suma el dinero recaudado por turno, analiza posibles anomalías transaccionales cruzando los registros lógicos y genera la liquidación financiera correspondiente.

---

## 🛠️ Instrucciones de Visualización y Edición

1.  **Edición:** Abre cualquiera de los archivos con extensión `.puml` listados en `image_338408.png` utilizando tu editor de código preferido (como VS Code).
2.  **Renderizado:** Asegúrate de contar con la extensión oficial de **PlantUML** instalada en tu entorno para procesar los scripts de actividades (`@startuml` / `@enduml`).
3.  **Previsualización:** Presiona la combinación de teclas `Alt + D` para procesar el código en tiempo real y exportar el diagrama estructurado en formato de imagen `.png`, quedando listo para anexarlo a la documentación técnica de **Synergy6**.

---

## 🖼️ Vistas Previas de los Diagramas

### Registro de Venta
![Registro de Venta](https://img.plantuml.biz/plantuml/png/dLJBJXj14BnRyZzqu68VeaHHoCCSWbaJX0H42b_GdctR3RFJcvuPIqZ-9GuH7n0f_h7qhAt48a2ad7PsfxgwfgfdZs92JRdn_TwBjA26eFN8eT-BDnnQL6nWx18lETqUexkPg-HGL-95OP_Uq8VPwqUXeZNf5lRs_S71ku_zNh-NE7c22UFSm0WrRGjgh4TGCQbI-LZXDS8jdFEtR5kEr_S11cErjqGkPKMua21-VPVOuR0Gh_RFURv8npxJQaAnHRV0sdeFAfERI8ShKraEsk-DhiIpuuJWVZTqfM5D7emyoE4EuwaIXTN5-hxENWfqLvIHZYe9CNjZMr98684274-WiXT5VxWBu31NYl8O1BtB7Y59GWzA3hCv8cQ1auOZIw1OSASKo0wlr8gcJdYhzDBlADf8Vyg1KPMBIAZPU0Hcwxl8JegUOi16R5E2V8XOnfsc7YB7H0rspNW6Wvy_JZmq4jAV2YSS7DVqQGWsLHRVrVhEaW8OZLlDD4NuIpR0CpvRuLUQMryJHvQakRDNPQpLLdjTEVb8CBYKhikJ5XZFMPS3RWKhcULRrOVT_abqobE2wnmJpsp2jWFu6Ir5utbr9LCjY-5_ofO0NwQHT6cm4ktUfk-4O-SzUj9K7Z39jFukdUMND1T36v92pRCkvkUciemsRiOPiDmn-STed3Mjijr-kr8tb0hdWu1YahPG79a0-rty0W00)

### Cierre de Caja
![Cierre de Caja](https://img.plantuml.biz/plantuml/png/ZLBDJXj13Bv7oZjOuf8SgjpJ2vkK8104bAL8bP0gCsiMbzcPOCzmgF92FUSHycBrR0gDMWvS_VFzsSUQK5Bk_72mERhWzZ7DVARDYJeAA1nXaOFZ6D33wAlcKXflXeD-QpYOdWLsZ52JycuRFbkbSeuQ0fllTjic-mWl519gwSsoEfpKvCdrcE0yMvDAxw2wbjXabsA_SnPQ8RLH38aRR4fj7iC3IuTxQAkyYR_cyBIPeqQusVro9Yx2g6PDPCEVu6PLBUllzRVb72vZY9vJRsQwO9yaWickgSrIQEx2wFAF_Yedes67hdWS6rs8YK0AtnHCYsQV46PVO6vpWjvsJ_Gv5qxRVHmRmssVWS7B2piw0Bz6nH-aC87zoB_m5xjjQzJ05fDODXIWeouAurrG3g3eBQWYNQWfHEXDla2Tedior4fBmgzHzdcLg_ulv9Gq5N-mok_8U7KvgLpAHl7JwFyQDkmLwJeR19RBBoIQt512x5t1YbexWc23S5vVBSU79_lGlqrlMVUy0YvszY7tk7ySJN4z71mRcptnRm00)
