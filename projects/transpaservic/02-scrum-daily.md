Volver al [inicio](../)

# 📝 **Proyecto Transpaservic**

## 🧑‍💻 **Visión General del Proyecto**

- **Nombre del Proyecto:** Transpaservic
- **Objetivo:** Desarrollar una sistema para la gestion de tiquetes.
- **Tecnologías:** NestJS, ReactJS, MySQL, cPanel, React Native.
- **Miembros del Equipo:**
  - David Lopez (Product Owner)
  - Frank GP (Scrum Master)
  - Felipe Hernández (Frontend Developer)
  - Frank GP (Backend Developer)
  - Ivana Barreto (UX/UI Designer)
- **Fecha de Inicio:** 13/enero/2025
- **Fecha de Finalización (MVP):** 13/febrero/2025
- **Fecha de Finalización (Proyecto):** 13/abril/2025

---

## 👥 **Roles**

### **Product Owner**

- **Nombre:** David Lopez
- **Responsabilidades:** Define funcionalidades clave, prioriza el backlog, gestiona expectativas del cliente.

### **Scrum Master**

- **Nombre:** Frank GP
- **Responsabilidades:** Facilita reuniones Scrum, elimina obstáculos, guía al equipo en prácticas ágiles.

### **Equipo de Desarrollo**

- **Nombres:**
  - Felipe Hernández (Frontend React)
  - Frank GP (Backend NestJS)
  - Ivana Barreto (Diseño UX/UI)
- **Responsabilidades:** Implementar funcionalidades, integrar diseño, asegurar calidad y rendimiento.

---

## 📦 **Product Backlog**

| ID  | Función/Tarea                           | Prioridad | Descripción                                       | Estado    |
| --- | --------------------------------------- | --------- | ------------------------------------------------- | --------- |
| 1   | Registro e inicio de sesión de usuarios | Alta      | Usuarios deben poder registrarse e iniciar sesión | Completo  |
| 2   | Gestion de Ordenes                      | Alta      | El administrador puede gestionar las ordenes      | Completo  |
| 3   | Gestion de Usuarios                     | Alta      | El administrador puede gestionar los usuarios     | Completo  |
| 4   | Gestion de Operadores                   | Alta      | El administrador puede gestionar los Operadores   | Completo  |
| 5   | Panel de administración                 | Media     | CRUD de ordenes, usuarios y operadores            | En curso  |
| 6   | Diseño responsive                       | Alta      | Adaptación móvil/tablet                           | Pendiente |
| 7   | Filtros de busqueda                     | Baja      | Filtros de busqueda de ordenes                    | Pendiente |

---

## 🧑‍💻 Sprints

## 🎨 Sprint 0: Diseño UI/UX y estructura visual

### Objetivo:

Tener todos los diseños listos en Figma para comenzar a desarrollar con una guía visual clara y consistente.

### Entregables:

- Sistema visual (tipografía, colores, botones, espaciado, iconografía).
- Prototipos de vistas principales (desktop y mobile).
- Documentación de componentes UI reutilizables.
- Flujo de navegación y experiencia de usuario.
- Link de Figma compartido con el equipo.

### Vistas a diseñar:

- [ ] Landing page / Home
- [ ] Registro e inicio de sesión
- [ ] Dashboard de operador (aprobar orden, subir tiquetes, etc.)
- [ ] Dashboard de administrador (gestión de usuarios, ordenes, etc.)

### Herramientas sugeridas:

- Figma (para diseño y prototipado)
- Notion / Trello / Jira (para vincular tareas con diseños)

---

## 🧱 **Sprint Backlog (Sprint 1)**

| ID  | Función/Tarea               | Prioridad | Descripción                                | Estado    |
| --- | --------------------------- | --------- | ------------------------------------------ | --------- |
| 1   | Registro e inicio de sesión | Alta      | Backend con JWT + Frontend con formularios | En curso  |
| 2   | Página de ordenes           | Alta      | Vista de ordenes desde la base de datos    | Pendiente |
| 3   | Diseño inicial y wireframes | Alta      | Mockups en Figma                           | Hecho     |

---

## 🗓 **Planificación del Sprint**

- **Duración del Sprint:** 1 semana
- **Meta del Sprint:** Tener login funcional y vista básica de ordenes
- **Fecha de Inicio:** 13/01/2025
- **Fecha de Finalización:** 20/01/2025

---

## 🔄 **Daily Scrum (Reuniones Diarias)**

### Día 2 - 02/05/2025

- **¿Qué hice ayer?**
  - Felipe: Comencé formulario de login
  - Frank: Implementé endpoint de login con JWT
- **¿Qué haré hoy?**
  - Felipe: Validar formulario e integrar con backend
  - Frank: Crear modelo de orden y seed inicial
- **¿Algún bloqueo?**
  - Felipe: Estoy esperando las credenciales de prueba

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
