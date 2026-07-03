# 🏷️ 6-Perfil — Diagrama de Perfil UML de TRANS-SYNC

Este directorio contiene los artefactos de modelado técnico para el **Diagrama de Perfil UML** del sistema **TRANS-SYNC**[cite: 1]. El objetivo de este módulo es definir extensiones personalizadas del metamodelo estándar de UML mediante estereotipos, propiedades y restricciones, adaptándolos específicamente al framework de desarrollo utilizado en el proyecto[cite: 1].

## 📂 Estructura del Directorio

Tal como se detalla en el árbol de archivos actual (ver `image_3393e3.png`), este directorio está compuesto por los siguientes recursos[cite: 1]:

* **📄 `perfil_springboot.puml`:** Script de PlantUML que define el perfil personalizado para Spring Boot, mapeando los conceptos propios de la arquitectura limpia y el ecosistema de microservicios sobre elementos estándar de UML[cite: 1].
* **📄 `Readme.md`:** Documentación guía del directorio actual[cite: 1].

---

## 🔍 Adaptación Tecnológica Modelada

El archivo `perfil_springboot.puml` representa la semántica técnica específica del desarrollo backend construida por **Synergy6** para guiar el diseño estructural de **TRANS-SYNC**[cite: 1]:

1. **Estereotipos de Componentes:** Define marcas semánticas personalizadas (como `«RestController»`, `«Service»`, y `«Repository»`) para clasificar de manera precisa las clases lógicas según su comportamiento dentro del framework[cite: 1].
2. **Inyección de Dependencias (DI):** Modela cómo se representan las anotaciones de gestión de inversión de control (como `«Autowired»` o `«Inject»`) sobre las relaciones lógicas del diagrama de clases[cite: 1].
3. **Persistencia y Entidades:** Introduce estereotipos especializados como `«Entity»`, `«Table»`, y `«Id»` para denotar componentes destinados al mapeo objeto-relacional (ORM) con las bases de datos lógicas independientes[cite: 1].

Este mecanismo de extensiones proporciona un vocabulario común unificado que permite a los diagramas estructurales del proyecto reflejar de manera exacta la implementación real en código fuente[cite: 1].

---

## 🛠️ Instrucciones de Visualización y Edición

1. **Edición:** Abre el archivo `perfil_springboot.puml` en tu editor de código preferido (como VS Code)[cite: 1].
2. **Renderizado:** Asegúrate de contar con la extensión oficial de **PlantUML** instalada en tu entorno de desarrollo para procesar la sintaxis de perfiles UML (`<<stereotype>>`, `profile`)[cite: 1].
3. **Previsualización:** Presiona la combinación de teclas `Alt + D` para procesar el código en tiempo real y exportar el diagrama estructurado en formato de imagen `.png`, quedando listo para incorporarlo formalmente a los manuales de desarrollo de la solución[cite: 1].+

https://img.plantuml.biz/plantuml/png/ZLJ1Rjf04BrRyZzCuL2YYYIAK9GYQeK0ju0gI0-LAaM3FNPMMNRTtNNKAE9Z-W4zvHFuiSxQa1YI2DONl3FptfkPXo-jG-EAXGo3J-wE5WIvHA72mDuBbQF11SGIhOMdC00-LnZVPqONAXbegGqqq_AiWzeaPDQ1qtddug8J1iim20Cdd2GO2imO4I4X-4uc5P8ij67qnv6oOlMim3D2t_mkXAFO5VmorahBrJydOeJMB3T2PSoZtP67_Gn3IeKISLcSa5p3Xa7EEZ4ZQFHwkT6UAOf-gLfzsGcff05DEa_FqjHtMBLHDSoL2t9OllZQGNdR-Z6-Xf5rgxygGNFK0BJWqwfeC-tuvmsGTMH8kyUyL34bwmPQEQEb95D26BxQZDYVBy3ISYsKwyBCUT5LRBa7UaRcGSHKObh-lOqfx8r1PJ5sGYkKNJy8IQWEmvvIhgrmsZok9UTwJyL8yTwhR58x_JcSIvhWWZvei9n8kyZRKMs-NUZroBibuPLKUMMN1-HvkOVaUQ5xqfQLzVgvP5FkMey1G28yY0IP4-jM_A2WTJFjJsRjsS_9e0lZrNDII0qZ5Uk5O4QqRB9c-jK_RonQozen5CMiUTjeKLJVmCPVy0qQ9vYB4th5QhnlY6kT2Ul_Y7MNISj4wujjXXstCP4p1RqF_Th8yAhIdymPjpBGDkoBSRnoDx-jwRuzEpqxtnNFapWs8hjpnv4NwtTPMDoicszUefxJX_c34LELKg9SCZX_8Vy3
