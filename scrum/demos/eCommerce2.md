Volver al [inicio](../)

# 📝 **Plantilla de Scrum - Proyecto eCommerce**

## 🧑‍💻 **Visión General del Proyecto**

- **Nombre del Proyecto:** TiendaOnline24
- **Objetivo:** Desarrollar una tienda en línea para vender productos de tecnología a nivel nacional.
- **Tecnologías:** NestJS, ReactJS, PostgreSQL, cPanel
- **Miembros del Equipo:**
  - Juan Pérez (Product Owner)
  - Carla Martínez (Scrum Master)
  - Luis Gómez (Frontend Developer)
  - Ana Torres (Backend Developer)
  - Sofía Ríos (UX/UI Designer)
- **Fecha de Inicio:** 01/05/2025
- **Fecha de Finalización (MVP):** 01/06/2025

---

## 👥 **Roles**

### **Product Owner**

- **Nombre:** Juan Pérez
- **Responsabilidades:** Define funcionalidades clave, prioriza el backlog, gestiona expectativas del cliente.

### **Scrum Master**

- **Nombre:** Carla Martínez
- **Responsabilidades:** Facilita reuniones Scrum, elimina obstáculos, guía al equipo en prácticas ágiles.

### **Equipo de Desarrollo**

- **Nombres:**
  - Luis Gómez (Frontend React)
  - Ana Torres (Backend NestJS)
  - Sofía Ríos (Diseño UX/UI)
- **Responsabilidades:** Implementar funcionalidades, integrar diseño, asegurar calidad y rendimiento.

---

## 📦 **Product Backlog**

| ID  | Función/Tarea                           | Prioridad | Descripción                                       | Estado    |
| --- | --------------------------------------- | --------- | ------------------------------------------------- | --------- |
| 1   | Registro e inicio de sesión de usuarios | Alta      | Usuarios deben poder registrarse e iniciar sesión | Pendiente |
| 2   | Página de productos                     | Alta      | Lista de productos disponibles con filtros        | Pendiente |
| 3   | Carrito de compras                      | Alta      | Agregar, editar y eliminar productos              | Pendiente |
| 4   | Pasarela de pago (simulada)             | Media     | Checkout básico con resumen de compra             | Pendiente |
| 5   | Panel de administración                 | Media     | CRUD de productos y usuarios                      | Pendiente |
| 6   | Diseño responsive                       | Alta      | Adaptación móvil/tablet                           | Pendiente |
| 7   | Reseñas de productos                    | Baja      | Los usuarios pueden dejar comentarios             | Pendiente |

---

## 🧱 **Sprint Backlog (Sprint 1)**

| ID  | Función/Tarea               | Prioridad | Descripción                                | Estado    |
| --- | --------------------------- | --------- | ------------------------------------------ | --------- |
| 1   | Registro e inicio de sesión | Alta      | Backend con JWT + Frontend con formularios | En curso  |
| 2   | Página de productos         | Alta      | Vista de productos desde la base de datos  | Pendiente |
| 3   | Diseño inicial y wireframes | Alta      | Mockups en Figma                           | Hecho     |

---

## 🗓 **Planificación del Sprint**

- **Duración del Sprint:** 1 semana
- **Meta del Sprint:** Tener login funcional y vista básica de productos
- **Fecha de Inicio:** 01/05/2025
- **Fecha de Finalización:** 07/05/2025

---

## 🔄 **Daily Scrum (Reuniones Diarias)**

### Día 2 - 02/05/2025

- **¿Qué hice ayer?**
  - Luis: Comencé formulario de login
  - Ana: Implementé endpoint de login con JWT
- **¿Qué haré hoy?**
  - Luis: Validar formulario e integrar con backend
  - Ana: Crear modelo de producto y seed inicial
- **¿Algún bloqueo?**
  - Luis: Estoy esperando las credenciales de prueba

---

## 🔍 **Revisión del Sprint**

- **Fecha:** 07/05/2025
- **¿Qué se hizo?**
  - Registro/Login funcional con JWT
  - Mockups de la tienda completados
- **Demo de entregables:**
  - Video de login en funcionamiento
  - Acceso al prototipo en Figma
- **Feedback del PO:**
  - Incluir opción de "Recuperar contraseña" en próximos sprints

---

## 📈 **Retrospectiva del Sprint**

- **Fecha:** 07/05/2025
- **¿Qué fue bien?**
  - Buena comunicación y entrega del diseño en tiempo
- **¿Qué se puede mejorar?**
  - Iniciar pruebas unitarias desde este sprint
- **Acciones para el siguiente sprint:**
  - Configurar Jest y pruebas básicas
  - Documentar endpoints en Swagger

---

## ✅ **Criterios de Hecho (Definition of Done)**

- Código aprobado por revisión
- Pruebas básicas implementadas
- Commit en repositorio con mensaje claro
- Documentación técnica actualizada
- Funcionalidad desplegada en entorno de pruebas
