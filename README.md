# 🐓 Sistema de Inventario – Granja El Milagro

Sistema web para la **gestión integral de inventario, producción, ventas, gastos y reportes** de una granja.  
Diseñado con **arquitectura escalable**, buenas prácticas y orientado a crecimiento futuro (multi-granja, app móvil, BI).

---

## 📌 Objetivo del Proyecto

Centralizar y digitalizar la información operativa de la granja para:
- Controlar animales y producción
- Registrar ingresos y egresos
- Analizar el estado económico
- Facilitar la toma de decisiones

---

## 👤 Usuarios del Sistema

| Rol | Descripción |
|---|---|
| Administrador | Control total del sistema |
| Operador (futuro) | Registro operativo |

---

## 🧩 Módulos del Sistema

### 🐓 1. Gestión de Animales
- Crear especies (pollos, gallinas, cerdos, peces, abejas)
- Registrar animales por lote o individuo
- Movimientos: entrada, salida, muertes
- Registro de peso y edad

---

### 🥚 2. Producción
- Registro de producción:
  - Huevos
  - Miel
  - Carne
- Datos diarios, semanales y mensuales
- Historial y acumulados

---

### 💰 3. Ventas
- Registro de ventas
- Productos vendidos
- Cantidad, precio y cliente
- Generación de comprobantes simples

---

### 🧾 4. Gastos
- Registro de gastos operativos
- Tipos:
  - Alimentación
  - Medicinas
  - Transporte

---

### 📊 5. Reportes
- Inventario actual
- Producción acumulada
- Balance económico
- Gráficos y estadísticas

---

## 🧠 Arquitectura del Sistema

Arquitectura **en capas (Clean Architecture / Modular)**:


---

## 🏗️ Stack Tecnológico

### Frontend
- React 18
- TypeScript
- Tailwind CSS

---

### Backend
- Node.js
- NestJS
- TypeScript
- Prisma ORM
- JWT Authentication
- Swagger (OpenAPI)

---

### Base de Datos
- PostgreSQL

---

### Infraestructura
- Docker
- Docker Compose
- Nginx

---

## 📁 Estructura del Repositorio
	backend/
├── src/
│   ├── modules/
│   │   ├── animal/
│   │   │   ├── animal.controller.ts
│   │   │   ├── animal.service.ts
│   │   │   ├── animal.module.ts
│   │   │   ├── dto/
│   │   │   │   ├── create-animal.dto.ts
│   │   │   │   └── update-animal.dto.ts
│   │   │   └── repository/
│   │   │       └── animal.repository.ts
│   │   │
│   │   ├── production/
│   │   │   ├── production.controller.ts
│   │   │   ├── production.service.ts
│   │   │   ├── production.module.ts
│   │   │   ├── dto/
│   │   │   │   ├── create-production.dto.ts
│   │   │   │   └── update-production.dto.ts
│   │   │   └── repository/
│   │   │       └── production.repository.ts
│   │   │
│   │   ├── sales/
│   │   │   ├── sales.controller.ts
│   │   │   ├── sales.service.ts
│   │   │   ├── sales.module.ts
│   │   │   ├── dto/
│   │   │   │   ├── create-sale.dto.ts
│   │   │   │   └── update-sale.dto.ts
│   │   │   └── repository/
│   │   │       └── sales.repository.ts
│   │   │
│   │   ├── expenses/
│   │   │   ├── expenses.controller.ts
│   │   │   ├── expenses.service.ts
│   │   │   ├── expenses.module.ts
│   │   │   ├── dto/
│   │   │   │   ├── create-expense.dto.ts
│   │   │   │   └── update-expense.dto.ts
│   │   │   └── repository/
│   │   │       └── expenses.repository.ts
│   │   │
│   │   ├── auth/
│   │   │   ├── auth.controller.ts
│   │   │   ├── auth.service.ts
│   │   │   ├── auth.module.ts
│   │   │   ├── strategies/
│   │   │   │   └── jwt.strategy.ts
│   │   │   └── guards/
│   │   │       └── jwt-auth.guard.ts
│   │   │
│   │   ├── users/
│   │   │   ├── users.controller.ts
│   │   │   ├── users.service.ts
│   │   │   ├── users.module.ts
│   │   │   ├── dto/
│   │   │   │   ├── create-user.dto.ts
│   │   │   │   └── update-user.dto.ts
│   │   │   └── repository/
│   │   │       └── users.repository.ts
│   │
│   ├── prisma/
│   │   ├── prisma.service.ts
│   │   └── schema.prisma
│   │
│   ├── common/
│   │   ├── filters/
│   │   │   └── http-exception.filter.ts
│   │   ├── interceptors/
│   │   │   └── response.interceptor.ts
│   │   ├── decorators/
│   │   │   └── roles.decorator.ts
│   │   ├── guards/
│   │   │   └── roles.guard.ts
│   │   └── constants/
│   │       └── roles.enum.ts
│   │
│   ├── config/
│   │   └── configuration.ts
│   │
│   ├── app.module.ts
│   └── main.ts
│
├── package.json
├── tsconfig.json
├── .env
└── README.md


---

## 🗄️ Modelo de Datos (Resumen)

### Entidades principales
- Usuario
- Especie
- Animal
- MovimientoAnimal
- Producción
- Producto
- Venta
- DetalleVenta
- Gasto

---



