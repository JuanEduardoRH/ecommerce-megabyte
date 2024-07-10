# Ecommerce - Megabyte - Finalizado

### [Ver demo](http://ecommerce-megabyte.typingideas.com)

usuario: admin@admin.com \
password: admin-ad

usuario: juan@cliente.com \
password: juan123


# Detalles

> Administrador:

En esta plataforma web, el administrador puede crear y modificar los productos que desee para poner a disposición toda la información necesaria para que estos mismos sean comprados por un cliente, esto se realiza mediante peticiones a una API REST creada en Laravel.

El administrador tendrá un módulo para gestionar todos los cupones, estos mismos aplicarán un descuento basándose en un porcentaje o un monto monetario en particular, limitando su uso en relación con una fecha de inicio, expiración y monto mínimo aceptado para aplicar dicho cupón. 

Para gestionar todos los pedidos realizados, existe un módulo el cual permite listar y filtrar todos los pedidos con base en cada etapa en la que se encuentre dicho pedido, todos los que se encuentren en este listado, tienen que haber sido pagados anteriormente, el administrador podrá ver el detalle en cada uno de ellos y actualizar a su siguiente estado respectivo en caso de ser necesario.

> Cliente:

La plataforma podrá a disposición todos los productos que se encuentren habilitados desde la administración para ser comprados, cada uno de ellos puede variar entre diferentes colores que puede tener, esto mismo no altera el valor del producto, para acceder a alguno de ellos, el cliente deberá realizar una búsqueda en la parte superior o acceder a alguno de los productos que aparecen en la pantalla principal.

Tendrá la facilidad de gestionar su carrito de compra en un menú lateral en todo momento, si así lo desea puede ver acceder a realizar la petición de sus productos en otra ventana, donde aparecerán los mismos detalles y la aplicación web, brindará la opción de agregar un cupón de descuento si así lo desea, para finalizar la compra, el cliente será redireccionado a WebPay, donde posterior al pago, será redireccionado a la página principal, dando inicio al proceso de preparación de su pedido.

El cliente podrá hacer seguimiento al estado de sus pedidos dentro de su panel personal, de esta manera estará al tanto de cuando está próximo a recibir los productos comprados.

## Dependencias del proyecto

La cantidad de dependencias puede ser mayor por el lado del front-end.

- Laravel 9
- Laravel Sanctum (Auth API)
- Transbank SDK
- Tailwind v3
- React v18
- React Query
- React Router
- React Cookie
- Framer Motion

## Otros
- Patrón repository

## Funcionalidades

- Administrador
  - Mantenedor de productos y filtro de búsqueda
  - Mantenedor de cupones, filtros de estados y búsqueda
  - Listado de pedidos
    - Filtro de búsqueda basándonos en el id
    - Filtro a base de estados
  - Ver detalle de pedido
  - Actualizar estado de pedido (hasta finalizar)
  - Edición de cuenta (Personal)
 
- Cliente
  - Listado de pedidos realizados
  - Ver detalle y estado de pedidos actuales
  - Agregar producto a su carrito
  - Ver detalles de su carrito (Menú lateral)
  - Ver listado de productos junto a detalle de pedido (checkout)
  - Agregar cupones a pedido actual
  - Pasarela de pago para concretar el pago de su pedido
  - Edición de cuenta (Personal)
