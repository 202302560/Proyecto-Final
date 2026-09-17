

# Sistema de Gestión de Inventarios y Compras

![Angular](https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white)

Plataforma web Full-Stack desarrollada para el **Supermercado Larry Cantillano**. Este sistema centraliza y automatiza el control de inventarios, la gestión de proveedores y el procesamiento de órdenes de compra, integrando un Dashboard analítico para la toma de decisiones en tiempo real.

---

## Características Principales (Módulos)

1.  Autenticación y Seguridad:** 
   - Sistema de login seguro con encriptación de contraseñas (`bcrypt`).
   - Protección de rutas y endpoints mediante JSON Web Tokens (`JWT`).
   - Control de acceso basado en roles (Administrador / Empleado).

2.  Gestión de Productos (CRUD):** 
   - Administración completa del catálogo de productos.
   - Definición de umbrales logísticos (Stock Actual vs. Stock Mínimo) para prevención de desabastecimiento.

3.  Gestión de Proveedores (CRUD):** 
   - Directorio unificado de aliados comerciales con información de contacto y direcciones.

4.  Órdenes de Compra:** 
   - Creación de pedidos asociando proveedores y múltiples productos.
   - **Automatización de Stock:** Uso de *Triggers* en PostgreSQL que actualizan y suman automáticamente el inventario físico al marcar una orden como "Completada".

5.  Dashboard Gerencial:** 
   - Tarjetas de métricas consolidadas (Total de productos, proveedores y órdenes).
   - Tabla reactiva con **Alertas de Stock Bajo** en tiempo real.
   - Gráficos de distribución estadística integrados con `Chart.js`.

---

## Tecnologías Utilizadas

* **Frontend:** Angular 17+ (Componentes Standalone), Bootstrap 5, Chart.js
* **Backend:** Node.js, Express.js
* **Base de Datos:** PostgreSQL (con lógica relacional y Triggers)
* **Seguridad:** JWT (jsonwebtoken), bcryptjs

---

## Requisitos Previos

Asegúrate de tener instalado lo siguiente en tu entorno de desarrollo:
* [Node.js](https://nodejs.org/) (v18 o superior)
* [Angular CLI](https://angular.io/cli) (`npm install -g @angular/cli`)
* [PostgreSQL](https://www.postgresql.org/) (v14 o superior)

---
