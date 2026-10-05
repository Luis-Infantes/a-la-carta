# FLOW AND SOFTWARE ARCHITECTURE

## FUNCTIONAL ARCHITECTURE 1

- The flow shown in this first diagram can be explained as follows:

1) Customers enter the restaurant and access the restaurant application through **Customer Menu**.
2) They place an order, which is then divided into two separate processes.
3) The table service and beverage management are handled through **Staff Command**.
4) Dish preparation management is carried out through **Kitchen Display**.
5) Once the dishes are confirmed, an alert is sent to the **Staff Command** application, which is responsible for collecting and serving the order.
6) Additionally, the solution includes an internal application called **Admin Management**, responsible for managing the restaurant's internal operations.

---

## FUNCTIONAL ARCHITECTURE 2

- In the following diagram, we continue showing part of the workflow:

1) When customers close an order to pay for it, two processes take place.
2) First, the order is closed, the data is archived, and it is used for future reports and statistics.
3) On the other hand, once the bill is closed, an invoice is generated to notify customers through the application of the amount that must be paid.

---

## FUNCTIONAL ARCHITECTURE 3

- This diagram shows the functionalities performed by the **Admin Management** application.

1) It is responsible for creating and editing the recipes that are available in the **Kitchen Display** application.
2) It also manages the creation and editing of the dishes displayed in the main menu.
3) From this application, users can manage statistics through a small chart embedded within the application itself.

---

## SOFTWARE ARCHITECTURE

- This diagram presents the technologies used in this project.

1) The solution is composed of four **Power Apps** applications.
2) All applications are connected to the same **SharePoint** site, where multiple lists store the data.
3) **Customer Menu** includes a **Power Automate** flow that runs whenever a new order is submitted.
4) **Staff Command** includes another **Power Automate** flow that is triggered when closed orders are archived in the database.


----------------------------------------


# ARQUITECTURA DE FLUJO Y DE SOFTAWARE


## ARQUITECTURA FUNCIONAL 1

- El flujo que mostramos en esta primera diapositiva se explica de la siguiente forma:

1) Clientes entran al local y acceden a la app del restaurante a traves de **Customer Menu**
2) Realizan su pedido, el cual se envía dividiéndose en dos partes.
3) La parte de inicio de mesa y bebidas se gestiona a través de **Staff Command**
4) La parte de gestión de platos se realiza a través de **Kitchen Display**
5) Una vez confirmados los platos, se envía una alerta a la aplicación de **Staff Command** que se encarga de recoger y servir
6) Además en la imagen contamos con otra aplicación interna llamada **Admin Management** que se encarga de gestionar la parte interna del restaurante.

----

## ARQUITECTURA FUNCIONAL 2

- En la siguiente diapositiva seguimos mostrando parte del flujo:

1) Los clientes cuando cierran una comanda para pagarla, suceden dos cosas
2) En primer lugar se cierra la comanda, los datos se archivan y se usan para futuros reportes y estadísticas
3) Por otra parte tras cerrar la cuenta se genera la factura para notificar a los clientes a traves de la app que tiene que abonar

----

## ARQUITECTURA FUNCIONAL 3

- En esta diapositiva mostramos las funciones que desempeña la app **Admin Management**

1) Se encarga de la creación y edición de las recetas de cocina que están disponibles en la app **Kitchen Display**
2) Además se encarga de la edición y creación de los platos que aparecen en el menú principal.
3) Desde esta app podremos gestionar las estadísticas con un pequeño grafico insertado en la propia app.

----

** ARQUITECTURA DE SOFTWARE

- En esta diapositiva veremos la tecnología empleada para este proyecto

1) La solución esta compuesta por cuatro aplicaciones en **Powwer App**
2) Todas están conectadas a un mismo sitio de Sharepoint, donde hay varias listas con datos
3) **Customer Menu** cuenta con un flujo de Power Automate cada vez que se envía una nueva comanda.
4) **Staff Command** cuenta con otro flujo de Power Automate que se activa cuando se archivan las comandas cerradas en la base de datos.
