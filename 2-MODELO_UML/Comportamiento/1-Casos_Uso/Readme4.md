# 👥 1-Casos_Uso — Especificación Funcional de TRANS-SYNC

Este directorio contiene los artefactos de modelado lógico para los **Casos de Uso** del sistema **TRANS-SYNC**, desarrollados bajo el estándar UML[cite: 1]. El objetivo de este módulo es representar las fronteras de la aplicación, los requerimientos funcionales del negocio y las interacciones de los distintos actores operativos con la plataforma de software[cite: 1].

## 📂 Estructura del Directorio

Tal como se detalla en el árbol de archivos actual (ver `image_05718a.png`), este módulo contiene los siguientes recursos esenciales[cite: 1]:

*   **📄 `casos_de_uso.puml`:** Script de PlantUML que consolida y agrupa los diferentes casos de uso del sistema[cite: 1].
*   **📄 `casos_uso_general.puml`:** Código fuente PlantUML que muestra la vista global de alto nivel, unificando a todos los actores de la empresa y sus interacciones principales con el software[cite: 1].
*   **📄 `casos_uso_pasajes.puml`:** Modelado específico centrado de forma exclusiva en la lógica y requerimientos funcionales del módulo de venta, reserva y control de pasajes interprovinciales[cite: 1].

---

## 🔍 Casos de Uso y Actores Core Modelados

Los scripts estructurados en este directorio reflejan los requerimientos de la empresa **Transportes Veloz Altiplano E.I.R.L.**[cite: 1]:

1.  **Módulo Pasajes (`casos_uso_pasajes.puml`):** Define el alcance de las acciones del *Despachador (Counter)* para seleccionar rutas entre Juliaca y Cusco, verificar la disponibilidad del mapa de los 7 asientos y emitir boletos[cite: 1].
2.  **Vista General (`casos_uso_general.puml`):** Consolida los flujos de los diferentes stakeholders del sistema (Despachador, Conductor, Pasajero y Dueño del negocio)[cite: 1].

---

## 🛠️ Instrucciones de Visualización y Edición

1.  **Edición:** Abre cualquiera de los archivos con extensión `.puml` listados en `image_05718a.png` utilizando tu editor de código preferido (como VS Code)[cite: 1].
2.  **Renderizado:** Asegúrate de contar con la extensión oficial de **PlantUML** instalada en tu entorno de desarrollo para compilar la sintaxis UML estándar de casos de uso (`actor`, `usecase`, `includes`)[cite: 1].
3.  **Previsualización:** Presiona la combinación de teclas `Alt + D` para procesar el código en tiempo real y exportar el diagrama como imagen `.png`, dejándolo listo para anexarlo a la documentación técnica final de **Synergy6**[cite: 1].

https://img.plantuml.biz/plantuml/png/PPB1Ji9048RlJVeE4ox20RmRGY0zcIW7AYGc9cJSZdN2TXTtPqtG-4YUV0HUp6sXGl7Mpdwp___txzGBEWcLJXDDBm9YmN7vAb2m8oLiJPhu3PijEgnWYsg39UMoqmJrEPfIKvgaYR34KORUUYW8bjx241uMitc-pX_d6VHdxYsmn9NW4EwjiNh_BQnmK6-Z4kkWj_G17TiUe8VZyzow2lKb0Iio1HNMFPb-7bHm7lLrHaOSwa6ptWBrxNz6ePUp5wgmuwmnmsBZucUQ00HF2ds4RmqhHWSvUTx_c8EjR7rdIpOTS45blDT5DCeAjc3pqW5N7Frh_eXaPgkjiyzeX5h-R9GcNxNppaU0uN1ofjycRCT7jJIvWWLfLB4wQhfWetHe4a3_vFIzncE7iHLoDNJ8wWzPOGSb6OfLgPEfM5Mh0wFHoGlSm7ZSg1GqcVo7pd9TejCO8lvylm00
https://img.plantuml.biz/plantuml/png/ZLLDJzj04Br7odyOSO4Sqjuh544TYYeLYX90wgaQrbDdothNx4SbLFK7zS2Xwa_87-jirX-n4w2dn3lFRzxCl1sVE8_MXrADHug-UV06h2nM7d9fINXfz7ZaxgMkq6895OfxB6Zf7nL1ZACk58r7uv6Nde_c4Wl68UG46JhZufyRP-2SD5bKC8NhnUdbShhySfd1qQbz2D8pJR085qORjNxoKk0aCgBmniB1FD3wZs4U1PTK627D0I3p1jAc0v5ZQIlC-U4eCq5xifE4wo8jEZCw3_7l1Y6QfpP-XGw_aqs9glgXZLuWisjPIj8-GShjaoYzxGmSR9UxbCvJkLrfh8jxuxnS_zKi-6Ty6-2mQrxWvXMfUUIOWefWPOxv9EA28u6EitpKKaYqi2GNcJQgRhAldqmXzLvA_abLkXxFBUcSR1rgMD9XEkkXCrDMbhE-DuhODv-rahfzgmwcs7CQphGmiMqvzdKigE1UHUu52Qf4BAgFRz9mNDv9smK62hKBYXqEP-pplAxx8P1lTIwG4n7Q-lWP6MUQGGK2mZnEIoDpravaZZhQSUolTX4yun_XbbRh9n6K6HPT6HkrRgPftdwGkdchgpP1ujbpIbEXr-lVGaU37MLOyYqcJZrfQ2w6XjrHUqwMD5jA3Goo31NP7z9j9gCztaaLtSX59Mda-bBZwxzYXaC6A1HHYOFvzgNSkg4mdSvs7RS7i6VgUr1xnjAJaNKtlrq2NORjJk-4NwDEMujLnJNLvumj6Q2lsXtJR9lcbS4j6ePtp3iW7WowjwWQZXqp7B81XGfvt3VN9cTJi5E1oaeHvXkBt946MQySbrOEn0y4h53m-d310RUEs77ZqM2Sy6RMRYPu1yV7CkMQpJRGdS6-Yk_6z5zGBkfbMAyTBs77enCMo5_EVm00
https://img.plantuml.biz/plantuml/png/XLJBRjim4BmBq3yiVAbzi7CF32E9uW0zk33YnDTY8ssKZMdI9QaYRj5FoYcVu1_hKfG4oGtGetPdPbz3NJcFrbTxbIQAdZru0vRB5my5Myez6vqcRiVwW1RtSC1yXoLj_54HX3pgKb6Qf8bdBw4CdN5G43mw0rDOdJwAIfaGMAF3Lt8mlhO_AlP2hIp2ocYZJk-USvm45SoziJ2w9IULNh2GZt5cAkt9JaQ03lBuqI6Zh3Lryj1y3BAM5CO6Icbjl6M75z-uUk9VauuKCA5yDn6CcjOlOKlQ8nmXCzfRetgpZE1t805KZd9qGXACgvGi56xP7Opc9rPSO158ruv5oRYww6Fs_QPoETe1_PvATju6ElfwZme60mejKq661ZnfiI0BDqQHhvUzPU6qZ9WT49PxzcpXWVCTULWg6TkUFZJdNPcO6f0s9BXS327zDSC0QLYnvf-eMsAJ6J3NrkGaMwvl82VKy83sbJosf13Fq1O3rieK_2p6i1VtTB2c5F-9n1s9B_wPiOT8ap_XAb_WQp0ArXrJt6NZ9351VTExqxkBncjS1TFfed-Qit2xoBFmeFRdXTUTCLkBdfSwZxUrebwkAXVLZh1yywJZLvfqI9ZD5Zrxm2NCvnnu1IqMd-3Q0_uFrrZa3DO7pcUp_WbhA8KUYyK2nXkM1rPYVNGVZpw9KybReJSMrzMv-603psfJotU2OIFzHtebqlA_-Wi0
