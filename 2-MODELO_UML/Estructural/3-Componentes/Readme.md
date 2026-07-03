# 🧩 3-Componentes — Diagramas de Componentes UML de TRANS-SYNC

Este directorio aloja el modelado técnico para los **Diagramas de Componentes UML** del sistema **TRANS-SYNC**. A diferencia del modelo C4 Nivel 3 enfocado en el backend, esta sección especifica la organización modular y estructural de las aplicaciones cliente, detallando las dependencias, subcomponentes e interfaces lógicas internas.

## 📂 Estructura del Directorio

De acuerdo con el árbol de archivos actual (ver `image_338fe3.png`), este módulo contiene los siguientes componentes esenciales:

* **📄 `componentes_app_movil.puml`:** Script de PlantUML que define la arquitectura interna, capas lógicas y dependencias del contenedor de la aplicación móvil.
* **📄 `Readme.md`:** Documentación e instrucciones guía del directorio actual.

---

## 🔍 Descripción del Modelo Móvil

El archivo `componentes_app_movil.puml` describe de manera gráfica los módulos internos que hacen funcionar la app móvil orientada a los conductores y gerencia de **Transportes Veloz Altiplano E.I.R.L.**:

1. **📱 Interfaz de Usuario (UI Layer):** Componentes lógicos de las vistas principales de la aplicación, como la pantalla de *Inicio de Ruta*, el *Mapa de Tracking* y el lector de escaneo de encomiendas.
2. **🧠 Control de Estado y Negocio (BLoC / Controllers):** Módulos internos encargados de gestionar las validaciones locales de datos en el teléfono antes de enviarlas al servidor central.
3. **🛰️ Servicios de Integración (API Services):** Componentes de red encargados de comunicarse directamente a través de HTTPS/JSON con el punto de control único (**API Gateway**).
4. **📍 Componentes de Hardware Nativo:** Controladores lógicos para interactuar con los recursos físicos del dispositivo móvil, tales como la geolocalización (GPS) para el rastreo del bus interprovincial en la carretera y la cámara para el escaneo de códigos QR de encomiendas.

---

## 🛠️ Instrucciones de Visualización y Edición

1. **Edición del Archivo:** Abre el archivo `componentes_app_movil.puml` utilizando tu entorno de desarrollo preferido (como VS Code).
2. **Renderizado de Código:** Asegúrate de tener activa la extensión oficial de **PlantUML** para compilar correctamente la sintaxis de interfaces y componentes estándar de UML.
3. **Previsualización:** Presiona las teclas `Alt + D` para procesar el archivo en tiempo real y exportar el esquema gráfico estructurado en formato `.png`, quedando listo para anexarlo a la sección de arquitectura del informe de **Synergy6**.

---

## 🖼️ Vista Previa del Diagrama

![Diagrama de Componentes de la App Móvil](https://img.plantuml.biz/plantuml/png/TL9DImCn5Bmlx7zuzkBsi0WUHOgb5bHi5RSYWY2FJTe6iqdCHrMaFwadVqB_c2-xNLgrNXPsCfcPDozdpgFreP9fSk3dlE9W90gL9kv5A8CMAoXrPRJYoXV-Gt8Wxd6Qf8aNdlxE1Sw8XC0u35eYTt0_keQS4CNVnVfBGTyO6As_5a92rhUlGNXU-c0HHbffkLvvKM8toXeiNt36eJD0Wp2G8kfru3DDO9i4EhjwvC92wRNbhji1T836Z3GTfSdohsJ1xK8mRI6RtFN7HLuyZWTD2k5rjtRwvKK-B4ZzfFh14q19opXJRLLfHkYyoGTWjAKBK1-PU13XvV-AGqKeZSZGjN84xLKZV4TCK2jsYYLDTVbSy5cmWY63xEfXqdGWMlSVp6izMwzS706oks7HScljMlbmipFwkBXJYR5DOCBIlh2Aom0ar6rr8qzIygR1D6dRXvpfDvNtcYXm0gUdmM6l1rV5pVZeOZAvBVQHu_pxkJ7TfZdgm-e5_w3cz6wIZ99mLSx3bDDhQeppTXErTBvfCatEw38zvcy0)
