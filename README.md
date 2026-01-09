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
	│   ├── api/
	│   │   ├── v1/
	│   │   │   ├── controllers/
	│   │   │   │   ├── animal.controller.js
	│   │   │   │   ├── production.controller.js
	│   │   │   │   ├── sales.controller.js
	│   │   │   │   ├── expenses.controller.js
	│   │   │   ├── routes/
	│   │   │   │   ├── animal.routes.js
	│   │   │   │   ├── production.routes.js
	│   │   │   │   ├── sales.routes.js
	│   │   │   │   ├── expenses.routes.js
	│   │   │   ├── validators/
	│   │   │   │   ├── animal.validator.js
	│   │   │   │   ├── production.validator.js
	│   │   │   │   ├── sales.validator.js
	│   │   │   │   ├── expenses.validator.js
	│   ├── config/
	│   │   ├── db.js
	│   │   ├── env.js
	│   ├── domain/
	│   │   ├── models/
	│   │   │   ├── Animal.js
	│   │   │   ├── Production.js
	│   │   │   ├── Sale.js
	│   │   │   ├── Expense.js
	│   │   ├── entities/
	│   │   │   ├── animal.entity.js
	│   │   │   ├── production.entity.js
	│   │   │   ├── sale.entity.js
	│   │   │   ├── expense.entity.js
	│   ├── services/
	│   │   ├── animal.service.js
	│   │   ├── production.service.js
	│   │   ├── sales.service.js
	│   │   ├── expenses.service.js
	│   ├── repositories/
	│   │   ├── animal.repository.js
	│   │   ├── production.repository.js
	│   │   ├── sales.repository.js
	│   │   ├── expenses.repository.js
	│   ├── utils/
	│   │   ├── errorHandler.js
	│   │   ├── response.js
	│   ├── app.js
	│   ├── server.js
	├── package.json
	├── .env

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



