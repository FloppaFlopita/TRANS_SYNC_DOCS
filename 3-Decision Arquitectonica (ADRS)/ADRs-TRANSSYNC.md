ADR 001: Uso de Arquitectura Monolítica para el Sistema TRANS-SYNC
Estado
Aceptado

Fecha
2026-07-02

Contexto
La empresa Transportes Veloz Altiplano E.I.R.L. requiere un sistema centralizado ("TRANS-SYNC") para conectar sus sedes físicas en Juliaca, Puno y Cusco con las unidades móviles en ruta. Actualmente, el negocio enfrenta problemas operativos graves derivados de procesos manuales: sobreventa de asientos en diferentes puntos, pérdida de trazabilidad en las encomiendas y un deficiente control de ingresos y liquidaciones.

Se necesita una solución de alta disponibilidad, pero que a la vez sea robusta, consistente y fácil de mantener. Si se optara por una arquitectura de microservicios, se añadiría una complejidad de infraestructura, latencia de red y costos operativos que no se justifican para el tamaño actual del equipo de desarrollo. Además, el sistema requiere transacciones de datos altamente consistentes (Ej. al registrar un pasaje y actualizar la caja al mismo tiempo), lo cual es mucho más complejo de lograr en sistemas distribuidos debido a las posibles inestabilidades de red en las rutas del Altiplano.

Decisión
Hemos decidido adoptar el estilo de Arquitectura Monolítica (específicamente un Monolito Modular) como base estructural del sistema TRANS-SYNC, fundamentado en los principios SOLID y el modelo C4.

El sistema se estructurará técnicamente en los siguientes pilares:

Punto de Entrada Unificado: Se prescinde de un API Gateway externo. Las peticiones de la Aplicación Web (Counter) y la Aplicación Móvil (Conductores/Dueño) se conectarán directamente a los endpoints expuestos por la aplicación central, pasando por un único filtro de seguridad (Módulo de Autenticación).

Módulos de Negocio Altamente Cohesivos: Dentro de la misma aplicación, el código se organizará en módulos o paquetes con responsabilidades únicas: Pasajes (rutas y asientos), Encomiendas (trazabilidad de carga), Autenticación (seguridad), Usuarios (perfiles y roles) y Liquidación (auditoría financiera).

Base de Datos Centralizada: Todos los módulos compartirán una única base de datos relacional. Para mantener el orden, se utilizarán esquemas lógicos o separación por tablas, aprovechando las capacidades transaccionales (ACID) del motor de base de datos para garantizar la integridad de la información.

Consecuencias

Positivas (Beneficios)

Simplicidad de Desarrollo y Despliegue: Al ser un solo artefacto (ej. un único archivo .jar), las pruebas, el despliegue en el servidor y el monitoreo son mucho más sencillos y económicos.

Rendimiento y Baja Latencia: La comunicación entre módulos (ej. Pasajes llamando a Liquidación) se realiza mediante invocaciones a métodos internos en la memoria RAM, eliminando por completo los tiempos de espera y fallos de las peticiones de red (HTTP/REST) que ocurren en los microservicios.

Consistencia Transaccional (ACID): Es mucho más fácil garantizar que si una venta falla, el registro de auditoría también se revierta automáticamente, ya que todo ocurre en la misma transacción de base de datos.

Negativas (Compensaciones / Trade-offs)

Punto Único de Fallo: Si existe un error crítico en un módulo (por ejemplo, un fallo de memoria al procesar un reporte), existe el riesgo de que toda la aplicación se detenga, afectando a las demás áreas del negocio.

Escalabilidad Global: Si el módulo de Pasajes requiere más recursos por alta demanda, se debe escalar (duplicar) la aplicación completa, no solo ese módulo específico.

Riesgo de Acoplamiento (Código Espagueti): Requiere una gran disciplina por parte del equipo de desarrollo para no mezclar las reglas de negocio entre los módulos, respetando las interfaces internas para no romper la estructura modular.