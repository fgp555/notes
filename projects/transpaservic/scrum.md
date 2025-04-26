# 📝 **Proyecto Transpaservic**

## 🧑‍💻 **Visión General del Proyecto**

- **Nombre del Proyecto:** Transpaservic
- **Objetivo:** Desarrollar una sistema para la gestion de tiquetes, usuarios, operadores.
- **Tecnologías:**
  - **Base de Datos:** MySQL
  - **Backend:** NestJS
  - **Frontend:** ReactJS
  - **Aplicación Móvil:** React Native
  - **Integraciones:** APIs de WhatsApp
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
  - **UX/UI Designer:** Ivana Barreto
  - **Frontend Developer:** Felipe Hernández
  - **Backend Developer:** Frank GP
  - **Auxiliar Frontend Developer:** Agustin Gerardo
- **Responsabilidades:** Implementar funcionalidades, integrar diseño, asegurar calidad y rendimiento.

---

## 📅 **Cronograma del Proyecto**

| Sprint       | Fecha de Inicio | Fecha de Finalización | Meta                                                                     |
| ------------ | --------------- | --------------------- | ------------------------------------------------------------------------ |
| **Sprint 0** | 13/01/2025      | 20/01/2025            | Análisis, diseño UI/UX, arquitectura de base de datos.                   |
| **Sprint 1** | 13/01/2025      | 20/01/2025            | Backend básico y frontend (registro, login, gestión de órdenes).         |
| **Sprint 2** | 27/01/2025      | 03/02/2025            | Desarrollo móvil (notificaciones push, visualización de órdenes).        |
| **Sprint 3** | 10/02/2025      | 17/02/2025            | Optimización y pruebas, validaciones de formularios, integración de API. |

---

## 📦 **Product Backlog**

| Función/Tarea                | Descripción                                              | Prioridad | Estado    |
| ---------------------------- | -------------------------------------------------------- | --------- | --------- |
| Registro e login de usuarios | Usuarios deben poder registrarse e iniciar sesión        | Alta      | Completo  |
| Gestion de Ordenes           | Crear tikets individuales                                | Alta      | Completo  |
| Gestion de Ordenes           | cargar múltiples tikets a través de archivos Excel       | Alta      | Completo  |
| Gestion de Ordenes           | Listado de tikets con filtros avanzados                  | Alta      | Completo  |
| Gestion de Ordenes           | Exportación de datos a Excel.                            | Alta      | Completo  |
| Gestion de Ordenes           | Consultas con opciones de exportación.                   | Alta      | Completo  |
| Gestion de Usuarios          | El administrador puede gestionar los usuarios            | Alta      | Completo  |
| Gestion de Operadores        | El administrador puede gestionar los Operadores          | Alta      | Completo  |
| Panel de administración      | CRUD de ordenes, usuarios y operadores                   | Media     | En curso  |
| Filtros de busqueda          | Filtros de busqueda de ordenes                           | Baja      | Pendiente |
| Envío de Emails              | En el registro de usuarios y recuperación de contraseñas | Media     | Pendiente |
| Envío de Emails              | Al crear nuevos tikets.                                  | Media     | Pendiente |
| Base de datos                | Creación y descarga de backups de la base de datos.      | Media     | Pendiente |
| Base de datos                | Respaldo de imágenes y archivos asociados.               | Media     | Pendiente |
| Funcionalidades del Frontend | Optimización y Compresión de Imágenes.                   | Media     | Pendiente |
| Funcionalidades del Frontend | Validación: Manejo de errores y predicción de texto.     | Media     | Pendiente |
| Funcionalidades del Frontend | Diseño responsive                                        | Media     | Pendiente |
| Funcionalidades del Frontend | Notificaciones web socket                                | Media     | Pendiente |
| Aplicación Móvil             | Notificaciones push                                      | Media     | Pendiente |
| DevOps                       | Implementación en servidores con cPanel                  | Media     | Pendiente |

---

## 🧑‍💻 Sprints

## 🎨 Sprint 0: Diseño UI/UX y estructura visual

### **Objetivo:** Análisis y Diseño (1 semana):

- Definición de requerimientos, diseño UI/UX, arquitectura técnica (diseño de la base de datos).
- Tener todos los diseños listos en Figma para comenzar a desarrollar con una guía visual clara y consistente.

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

# 🧱 Sprint Backlog

## 🧱 **Sprint 1** Backend & Frontend

| Función/Tarea               | Descripción                                | Prioridad | Estado    |
| --------------------------- | ------------------------------------------ | --------- | --------- |
| Diseño inicial y wireframes | Mockups en Figma                           | Alta      | Hecho     |
| Registro e inicio de sesión | Backend con JWT + Frontend con formularios | Alta      | En curso  |
| Página de ordenes           | Vista de ordenes desde la base de datos    | Alta      | Pendiente |

### **Planificación del Sprint**

- **Duración del Sprint:** 4 semanas
- **Meta del Sprint:** Creación de APIs, validaciones, autenticación y seguridad.
- **Fecha de Inicio:** 13/01/2025
- **Fecha de Finalización:** 20/01/2025

## 🧱 **Sprint 2** Mobile

| Función/Tarea               | Descripción                                | Prioridad | Estado    |
| --------------------------- | ------------------------------------------ | --------- | --------- |
| Diseño inicial y wireframes | Mockups en Figma                           | Alta      | Hecho     |
| Registro e inicio de sesión | Backend con JWT + Frontend con formularios | Alta      | En curso  |
| Página de ordenes           | Vista de ordenes desde la base de datos    | Alta      | Pendiente |

### **Planificación del Sprint**

- **Duración del Sprint:** 4 semanas
- **Meta del Sprint:** Tener login funcional y vista básica de ordenes
- **Fecha de Inicio:** 27/01/2025
- **Fecha de Finalización:** 03/02/2025

## 🧱 **Sprint 3** Pruebas y Optimización

| Función/Tarea               | Descripción                                | Prioridad | Estado    |
| --------------------------- | ------------------------------------------ | --------- | --------- |
| Diseño inicial y wireframes | Mockups en Figma                           | Alta      | Hecho     |
| Registro e inicio de sesión | Backend con JWT + Frontend con formularios | Alta      | En curso  |
| Página de ordenes           | Vista de ordenes desde la base de datos    | Alta      | Pendiente |

### **Planificación del Sprint**

- **Duración del Sprint:** 2 semanas
- **Meta del Sprint:** Validación del sistema, corrección de errores y mejora del rendimiento.
- **Fecha de Inicio:** 10/02/2025
- **Fecha de Finalización:** 17/02/2025

## 🧱 **Sprint 4** Entrega Final y Capacitación

| Función/Tarea               | Descripción                                | Prioridad | Estado    |
| --------------------------- | ------------------------------------------ | --------- | --------- |
| Diseño inicial y wireframes | Mockups en Figma                           | Alta      | Hecho     |
| Registro e inicio de sesión | Backend con JWT + Frontend con formularios | Alta      | En curso  |
| Página de ordenes           | Vista de ordenes desde la base de datos    | Alta      | Pendiente |

### **Planificación del Sprint**

- **Duración del Sprint:** 1 semana
- **Meta del Sprint:** Validación del sistema, corrección de errores y mejora del rendimiento.
- **Fecha de Inicio:** 10/02/2025
- **Fecha de Finalización:** 17/02/2025

---

---

---

---

# 🏃‍♂️ Sprint 2

- **Fecha de Inicio:** 27/enero/2025
- **Fecha de Finalización:** 10/febrero/2025
- **Objetivo del Sprint:** Finalizar la gestión de usuarios, operadores y completar el panel de administración básico.

## ✅ Historias de Usuario y Tareas

| Historia/Tarea          | Descripción                                                                 | Estado      |
| :---------------------- | :-------------------------------------------------------------------------- | :---------- |
| Gestión de Usuarios     | Crear, editar, eliminar y listar usuarios desde el panel de administración. | En progreso |
| Gestión de Operadores   | Crear, editar, eliminar y listar operadores.                                | En progreso |
| Panel de Administración | Implementar CRUD de órdenes, usuarios y operadores.                         | En progreso |

## 🎯 Entregables

- CRUD de usuarios funcionando.
- CRUD de operadores funcionando.
- Sección inicial del panel administrativo operativa.

---

# 🏃‍♂️ Sprint 3

- **Fecha de Inicio:** 10/febrero/2025
- **Fecha de Finalización:** 24/febrero/2025
- **Objetivo del Sprint:** Integrar funcionalidades de envío de correos y filtros de búsqueda en órdenes.

## ✅ Historias de Usuario y Tareas

| Historia/Tarea      | Descripción                                                 | Estado    |
| :------------------ | :---------------------------------------------------------- | :-------- |
| Envío de Emails     | Al registrar nuevos usuarios y recuperación de contraseñas. | Pendiente |
| Envío de Emails     | Notificación automática al crear nuevos tiques.             | Pendiente |
| Filtros de Búsqueda | Implementar filtros avanzados en la vista de órdenes.       | Pendiente |

## 🎯 Entregables

- Funcionalidad de recuperación de contraseña vía correo.
- Correos de notificación automática de creación de tickets.
- Filtros funcionales en la búsqueda de órdenes.

---

# 🏃‍♂️ Sprint 4

- **Fecha de Inicio:** 24/febrero/2025
- **Fecha de Finalización:** 10/marzo/2025
- **Objetivo del Sprint:** Mejoras en Frontend, backups de base de datos y archivos.

## ✅ Historias de Usuario y Tareas

| Historia/Tarea           | Descripción                                                      | Estado    |
| :----------------------- | :--------------------------------------------------------------- | :-------- |
| Optimización de Imágenes | Comprimir imágenes subidas a la plataforma.                      | Pendiente |
| Validaciones Frontend    | Manejo de errores, predicción de texto, formularios más seguros. | Pendiente |
| Diseño Responsive        | Adaptar el diseño a distintos dispositivos.                      | Pendiente |
| Backups de Base de Datos | Creación y descarga de respaldos.                                | Pendiente |
| Backups de Archivos      | Respaldo de imágenes y archivos adjuntos.                        | Pendiente |

## 🎯 Entregables

- Frontend optimizado y adaptativo.
- Funcionalidades de backup operativas en el sistema.
