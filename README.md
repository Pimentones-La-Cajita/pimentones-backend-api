# ⚙️ Pimentones La Cajita · Backend API & Microservicios

Núcleo transaccional de la plataforma, desarrollado en **NestJS 11** sobre **Fastify**, con **Drizzle ORM**, base de datos relacional **PostgreSQL 16** y worker asíncrono.

## 🏛️ Dominios y Endpoints
* **Catálogo:** /api/products (listado, slug, precios, maridajes).
* **Pedidos & Checkout:** /api/orders (cotización de flete, creación atómica, tracking).
* **Pasarelas de Pago:** /api/payments/wompi/events (webhook seguro con validación SHA-256).
* **Backoffice API:** /api/admin/* (dashboard, órdenes, inventario, zonas, cupones).
* **Asistente IA:** /api/assistant/chat (recomendador de conservas).
* **Worker en Cola:** Procesamiento de correos SMTP y expiración de órdenes pendientes.

## 🗄️ Base de Datos
* PostgreSQL 16 en contenedor Docker (localhost:5434).
* 14 tablas relacionales con migraciones SQL automáticas al arrancar.

## 🚀 Inicio Rápido
``bash
npm install
npm run dev
``
* API REST: [http://localhost:4001/api](http://localhost:4001/api)
* Documentación Swagger: [http://localhost:4001/api/docs](http://localhost:4001/api/docs)
