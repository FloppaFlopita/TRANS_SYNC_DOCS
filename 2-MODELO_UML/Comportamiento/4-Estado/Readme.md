# 🏁 4-Estado — Diagramas de Estado de TRANS-SYNC

Este directorio contiene los artefactos de modelado técnico para los **Diagramas de Estado** del sistema **TRANS-SYNC**, desarrollados bajo el estándar UML. El objetivo de este módulo es representar el ciclo de vida de las entidades críticas del negocio, detallando los diferentes estados por los que pasan y los eventos o transiciones que provocan dichos cambios.

## 📂 Estructura del Directorio

Tal como se detalla en el árbol de archivos (ver `image_3384a2.png`), este directorio está compuesto por los siguientes recursos:

* **📄 `est_encomienda.puml`:** Script de PlantUML que define el ciclo de vida y las transiciones lógicas de una encomienda (paquete/carga) dentro del flujo logístico.
* **📄 `Readme.md`:** Documentación guía del directorio actual.

---

## 🔍 Ciclo de Vida del Negocio Modelado

El diagrama contenido en este módulo especifica de forma exacta el comportamiento dinámico de la entidad principal de logística para **Transportes Veloz Altiplano E.I.R.L.**:

### Estados de una Encomienda (`est_encomienda.puml`):
1.  **📦 Registrado / Recibido:** El paquete es pesado, cotizado y se genera su código QR único en el counter de origen (Juliaca o Cusco).
2.  **🚚 En Almacén de Salida:** La carga se encuentra resguardada en la terminal esperando la asignación de la unidad móvil de transporte.
3.  **🚌 Transitando / En Ruta:** El conductor ha iniciado el viaje y el paquete se encuentra físicamente dentro del bus interprovincial.
4.  **🏢 En Almacén de Destino:** La unidad llega a la terminal de llegada y el paquete es descargado, quedando listo para ser recogido por el destinatario.
5.  **✅ Entregado:** El cliente final retira el paquete mediante la validación del código QR y la firma de conformidad, finalizando el ciclo de vida de la entidad.
6.  **⚠️ Incidencia / Devuelto (Si aplica):** Estado alternativo en caso de pérdidas, daños o si el paquete no es reclamado en el tiempo límite establecido.

---

## 🛠️ Instrucciones de Visualización y Edición

1.  **Edición:** Abre el archivo `est_encomienda.puml` en tu editor de código preferido (como VS Code).
2.  **Renderizado:** Asegúrate de contar con la extensión oficial de **PlantUML** instalada en tu entorno de desarrollo para compilar la sintaxis de transiciones de estado (`[*] --> Estado`).
3.  **Previsualización:** Presiona la combinación de teclas `Alt + D` para procesar el código en tiempo real y exportar el diagrama estructurado en formato de imagen `.png`, dejándolo listo para anexarlo a la documentación técnica final de **Synergy6**.

---

## 🖼️ Vista Previa del Diagrama

![Estado de una Encomienda](https://img.plantuml.biz/plantuml/png/VPB1RjD048RlblmEmwr5HDmve5g95GKH1nnJ2H4K3Ukf6LZFkklTI0ZnI7sAlbXd4xUgMi2NiMPtllrd_haO0_eGUvjdBy9twWa6YonvbcU1WoMOix4EMe9BRZ75A0Yb6DSpYMRE2dyTEP09qIEidJXxUnFOu3dCeAcBQZlRVgxc2VZbvLUOpTv2MUsBz-jYhd5JhvPb1MzWxg84yk2fup4eQS3hI85sShOa8KryhE4ND1xDJvRkFF6USoPw_QafZanfemdE0uxSgMo3liET_bY4deKFACeST02KU3gAG0_rl_CCz7iGBVjBnX-qNoMTWtS75iDeJxV-TNeiLT4oVdE-TVko9zzHEb9zDGrEdqv3nGFvsnlLHf9KUktSumdzz-h_IKgjfqwXrunQf5YNHZgrd6T_fkaT-tpYoABSDgjgeuprD25hILa88xN9ZdVHCXg4r_0XYjCmZwDnJmsvnvpeJLqkYyNcaS_QBr_fbi2YMhtQoHNx7jKBak3JQvFx9-XzTMAf7NbsePkdAti7)
