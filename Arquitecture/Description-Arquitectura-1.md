## Arquitectura Funcional

### Descripción

Este diagrama representa la arquitectura funcional de la solución y muestra cómo interactúan las distintas aplicaciones que forman parte del ecosistema. La función principal del sistema es gestionar el ciclo completo de un pedido, desde la selección realizada por el cliente hasta su preparación y gestión administrativa.

La arquitectura está basada en varias aplicaciones independientes, cada una especializada en una fase concreta del proceso de negocio, permitiendo distribuir responsabilidades entre clientes, personal de cocina, personal de sala y administración.

---

### Componentes Principales

#### Customer Menu

Aplicación utilizada por los clientes para consultar la oferta disponible y realizar pedidos.

Funciones principales:

- Visualización del catálogo.
- Selección de productos.
- Generación de pedidos.
- Inicio del flujo operativo del sistema.

---

#### Sistema de Pedido

Elemento central que representa la generación y gestión inicial de los pedidos realizados por los clientes.

Este componente actúa como punto de distribución de la información hacia las aplicaciones operativas encargadas de gestionar la preparación y supervisión de los pedidos.

---

#### Kitchen Display

Aplicación destinada al personal de cocina.

Funciones principales:

- Recepción de pedidos entrantes.
- Visualización del estado de preparación.
- Seguimiento de tareas de cocina.
- Comunicación con el sistema de supervisión.

---

#### Staff Command

Aplicación utilizada por el personal operativo o de supervisión.

Funciones principales:

- Supervisar pedidos activos.
- Coordinar la atención al cliente.
- Gestionar incidencias operativas.
- Realizar el seguimiento del servicio.

---

#### Admin Management

Aplicación enfocada a tareas de administración y gestión.

Funciones principales:

- Gestión global del sistema.
- Supervisión de operaciones.
- Control administrativo.
- Consulta de información operativa.

---

### Flujo de Funcionamiento

1. Los clientes acceden a la aplicación **Customer Menu**.
2. El cliente realiza un pedido utilizando la aplicación.
3. El pedido generado es enviado al sistema central.
4. El sistema distribuye la información simultáneamente a:
   - La aplicación **Kitchen Display** para la preparación.
   - La aplicación **Staff Command** para la supervisión del servicio.
5. Kitchen Display proporciona información operativa al sistema de administración.
6. Staff Command supervisa el estado de los pedidos y coordina la entrega.
7. Una vez completado el proceso, los clientes reciben el servicio solicitado.

---

### Objetivo de la Arquitectura

El objetivo principal de esta arquitectura funcional es desacoplar las responsabilidades operativas en varias aplicaciones especializadas, permitiendo que cada perfil de usuario interactúe únicamente con la información necesaria para sus funciones.

Este enfoque mejora:

- La organización de los procesos.
- La escalabilidad de la solución.
- La experiencia de usuario.
- La coordinación entre las áreas operativas y administrativas.
- La capacidad de mantenimiento y evolución futura del sistema.
