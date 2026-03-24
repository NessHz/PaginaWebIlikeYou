# Sistema de Ecommerce con Gestión de Ventas y Delivery (Laravel)

Aplicación web desarrollada con Laravel que implementa un sistema de ecommerce con gestión de usuarios, control de inventario, validación de ventas y coordinación de entregas mediante múltiples roles.

## Descripción

Este proyecto simula el funcionamiento de una tienda online donde el proceso de compra incluye validación manual por parte de un asesor de ventas y coordinación con un sistema de delivery. El sistema está diseñado para representar un flujo de negocio realista basado en pedidos gestionados a través de WhatsApp.

## Características principales

- Autenticación de usuarios con registro, login y verificación por correo  
- Sistema de roles con permisos diferenciados  
- Catálogo de productos con categorías y ofertas  
- Carrito de compras y lista de favoritos  
- Integración con WhatsApp para generación de pedidos  
- Gestión de pedidos y estados  
- Generación de comprobantes de venta  
- Persistencia de datos con MySQL  

## Roles del sistema

### Cliente
- Navegación del catálogo  
- Gestión de carrito y favoritos  
- Generación de pedidos vía WhatsApp  

### Asesor de ventas
- Recepción y validación de pedidos  
- Confirmación de pago  
- Actualización del estado del pedido  

### Administrador de inventario
- Gestión de productos  
- Gestión de categorías  
- Configuración de ofertas  

### Administrador general
- Gestión de usuarios  
- Asignación y modificación de roles  
- Control total del sistema  

### Delivery
- Visualización de pedidos confirmados  
- Marcado de pedidos como entregados  
- Registro de evidencia de entrega  

## Flujo de compra

1. El cliente navega por el catálogo y agrega productos al carrito  
2. Se genera un pedido a través de WhatsApp  
3. El asesor de ventas valida el pedido manualmente  
4. El pedido es marcado como pagado y confirmado  
5. El pedido pasa al módulo de delivery  
6. El delivery realiza la entrega y registra evidencia  
7. Se genera un comprobante de la transacción  

## Tecnologías utilizadas

- Laravel  
- PHP  
- MySQL  
- Blade  
- Bootstrap  
- JavaScript  

## Estructura del proyecto

/routes → Definición de rutas  
/app → Lógica de negocio (controladores, modelos)  
/resources/views → Vistas Blade  
/database → Migraciones y seeders  
/public → Archivos públicos y assets  

## Instalación

Clonar el repositorio:

git clone https://github.com/tu-usuario/tu-repo.git

Instalar dependencias:

composer install

Configurar entorno:

cp .env.example .env  
php artisan key:generate  

Configurar la base de datos en el archivo .env y ejecutar:

php artisan migrate  

Iniciar servidor:

php artisan serve  

## Capturas

Pendiente de agregar capturas del sistema

## Mejoras futuras

- Despliegue en entorno productivo  
- Integración con pasarela de pagos  
- Notificaciones en tiempo real  
- Mejora de interfaz de usuario  
- API REST para integración externa  

## Autor

Sebastián Huertas  
Estudiante de Ingeniería Informática