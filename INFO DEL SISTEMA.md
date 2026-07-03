# TRANS-SYNC

¡Bienvenido al repositorio oficial de **TRANS-SYNC**, una solución integral de software basada en microservicios diseñada para optimizar y gestionar los procesos operativos, comerciales y financieros de las empresas de transporte interprovincial.

Este proyecto ha sido desarrollado por el startup **Synergy6** para la Escuela de Ingeniería de Sistemas de la Universidad Peruana Unión (UPeU) - Campus Juliaca.

## 🚀 Integrantes de Synergy6
* Christian Yoel Soncco Vargas – 202320719
* Edgar D'Alessandro Cabana Cruz - 202420888
* Soncco Cruz Fidel Edison – 202320600
* Ramos Ancco Alexander – 202411747
* Anghelo Hernan Torres Arias - 202420887

---

## 📋 Descripción del Proyecto

**TRANS-SYNC** es una plataforma moderna orientada a resolver las ineficiencias de comunicación, duplicidad de datos y falta de automatización en el sector de transporte terrestre. El sistema descompone la complejidad del negocio en microservicios independientes, garantizando alta disponibilidad, escalabilidad y tolerancia a fallos.

### Módulos Principales
1. **Pasajes (Ventas):** Gestión de rutas, asignación de buses en tiempo real, reservas y emisión de boletos de viaje.
2. **Encomiendas:** Control completo del ciclo de vida de los envíos, pesaje, tarifas y generación de códigos QR para el rastreo y tracking logístico.
3. **Seguridad (Autenticación):** Control de accesos y seguridad perimetral mediante JWT y roles (Administrador, Conductor, Cajero, Pasajero).
4. **Usuarios:** Centralización y gestión del perfil de empleados, clientes y conductores.
5. **Liquidación (Caja/Auditoría):** Auditoría financiera, control de cierres de caja por terminal y detección automatizada de anomalías en las transacciones de ventas.

---

## 🏗️ Enfoque Arquitectónico (Modelo C4)

El sistema implementa una arquitectura desacoplada basada en **Monolito** comunicados a través de un **API Gateway**. Cada microservicio cuenta con su propia persistencia de datos (**Database-per-Service**) utilizando **PostgreSQL**.

### Tecnologías Clave:
* **Backend:** Java, Spring Boot, Spring Cloud (Gateway, Eureka / Config Server)
* **Persistencia:** PostgreSQL, Spring Data JPA
* **Contenedores:** Docker, Docker Compose
* **Diagramación/Modelado:** PlantUML (Modelo C4 - Niveles 1, 2 y 3)

---

## 🛠️ Requisitos Previos

Antes de levantar el proyecto de manera local, asegúrate de tener instalado:
* **Java JDK 17** o superior
* **Maven 3.8+**
* **Git**