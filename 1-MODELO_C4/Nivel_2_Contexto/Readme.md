Nivel 2: Diagrama de Contenedores — TRANS-SYNC (Monolito)Este directorio alberga el diseño de Nivel 2 (Contenedores) bajo el enfoque del Modelo C4, detallando la estructura del sistema TRANS-SYNC bajo una Arquitectura Monolítica. En este nivel se define la distribución centralizada de la plataforma, donde las aplicaciones frontales se comunican directamente con un único servidor backend que gestiona una base de datos unificada.

## 🔍 Descripción de los Contenedores Centrales

El modelado describe los componentes de software clave que integran el ecosistema operativo de la empresa[cite: 1]:

1.  **💻 App Web (Terminales):** Contenedor desarrollado en React/Angular enfocado en los counters para una venta ágil de boletos y recepción de carga[cite: 1].
2.  **📱 App Móvil (Operadores):** Herramienta móvil en Flutter/React Native orientada al uso de choferes en ruta y visualización gerencial[cite: 1].
3.  **🛡️ API Gateway:** Punto único de entrada al sistema que gestiona de manera centralizada la seguridad, el ruteo dinámico mediante HTTPS/JSON y la validación perimetral de tokens JWT[cite: 1].
4.  **⚙️ Microservicios Core Backend:**
    *   **Servicio Pasajes:** Gestión lógica de asientos y control estricto de rutas interprovinciales[cite: 1].
    *   **Servicio Encomiendas:** Módulo dedicado a la trazabilidad y la logística de almacenamiento de paquetes[cite: 1].
    *   **Servicio Auth:** Gestión integral de sesiones, permisos y emisión de credenciales de seguridad[cite: 1].
    *   **Servicio Liquidación:** Motor de auditoría encargado del control de flujos de dinero y cierres de caja financieros[cite: 1].

---

## 🛠️ Visualización y Renderi   zado

Para previsualizar o compilar los diagramas:
1. Abre `c4_nivel2_containers.puml` o `arquitectura_microservicios.puml` en VS Code[cite: 1].
2. Asegúrate de tener activa la extensión de **PlantUML**[cite: 1].
3. Presiona `Alt + D` para procesar el código de diseño y exportarlo directamente en un archivo de imagen (`.png`)[cite: 1].

![]https://img.plantuml.biz/plantuml/png/bLF1Jjj04BrRyZ-Cu98SSYed3XMEeU9GK4I2gWhbC7WdTCjwnvtTHPMgV59FV49-h6DZ0X46fMl9MkdDl3VlZNqI8afCjSipHwi8aK7itOy8nWfLqRBFit1lVOE2DNWs17_o3FHCiRg_4qxUbEnOu71rr3uzo698Uk1JT_9idMTv5crq18Mdtmpdnt15ZL0W7x6ocqSF5VkAcfZGmQYGNyb6dI89mWLxTfk_qLOuRdcwKGvAPxMN0eo-2El5c_71yu0tHTF0Dxg5qOAajXuTXV7o5NQnUNomgbEoDwcAB4_u-eL-Jl9WZNeeLKNQcLhNEofzeGsHQeJ5LN4vdyo_NvRRWavEfKno34NI6LiFdTlbGCLrI2YMmn0smu0_QH0wynNNceN1GVYhrIZDZkgwTsemuYq6DJ5jt-hc52C7kFPsfOCQt3ePJK-tGRmO7VSymt73PF8PRjx6iuHZc94ceL-OhkzyiPZr58DR-IyQ9NedxuxcNHjlTx1d_VDUzYn_lQizMtRszt5FdfqejVxH_m00
https://img.plantuml.biz/plantuml/png/bPF1Qjj048Rl0ht3rBt846EIfgtneSIndROXSLtBePGwX95sAc-psXMxg-HG-aWz53-2NwmZoR63mOKA8QJTVxwP-MTrvZnQN-Og35xu9UK4XKAfmy3TIrsWnHmifHvrfWX-XW7mTOxfVMPDgSNGA6FXvUchdX2lcyqBetsp_BYKdZOHnWgo6_NnyPjU8iBWr_Ca0Zqcw0xdE4dUzkZqG0v6XO6NdckSo0TISDA7aSICoGY2OCW1f4aOImuwC9yD9d4d_ZePGdHjj57IctQ5mDGpj3KYLs2wHDQt01qJjjzR3ID5MRzsOLJI-e-ffRbvaEgkT6Ghtiwwrg1GCiLKhbSQlb02qPniBZKgSks5_hQhi0ypuXpTWSvAXVQsnZvISf1slLvnpZt6XIgz9yiKOOqK3GMBuXzLrKwiVtjUUERG7ZSkhDGP3zJusuLUwFVal3GQmHk1eFXUhxAAmAvhoamgpK97Wz8lZs2A3d-GEuAnJaqkIGjqxOrhpH2gwhOdeNLUFPapGcySt6ZvdS42kQAfSJwp57--QXfBn5rAsbjKDM4tBkXqtbNcGHzk74BqOJwVnZpgtPXg1HkphmY3AgpQV2gE5LDYTxXTFaM3wKUOZUCvH9VnfqdtAQmY_NTGLSz6NiNkkk7eAwBksALM9WGHDypoCtQE_zY_` 
