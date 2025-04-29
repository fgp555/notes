# 📝 **Proyecto Transpaservic**

## 🧑‍💻 **Visión General del Proyecto**

- **Nombre del Proyecto:** Transpaservic
- **Objetivo:** Desarrollar una sistema para la gestion de tiquetes, user, operator.
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

| Función/Tarea   | Descripción                                                  | Prioridad |
| --------------- | ------------------------------------------------------------ | --------- |
| Database        | Creación y descarga de backups de la base de datos.          | Media     |
| Database        | Respaldo de imágenes y archivos asociados.                   | Media     |
| DevOps          | Implementación en servidores con cPanel                      | Media     |
| Frontend        | Diseño responsive                                            | Media     |
| Frontend        | Notificaciones web socket                                    | Media     |
| Frontend        | Optimización y Compresión de Imágenes.                       | Media     |
| Frontend        | Validación: Manejo de errores y predicción de texto.         | Media     |
| Mobile          | Notificaciones push                                          | Media     |
| Module operator | El administrador puede gestionar los operator                | Alta      |
| Module order    | cargar múltiples tikets a través de archivos Excel           | Alta      |
| Module order    | Consultas con opciones de exportación.                       | Alta      |
| Module order    | Crear tikets individuales                                    | Alta      |
| Module order    | Exportación de datos a Excel.                                | Alta      |
| Module order    | Filtros de busqueda de order                                 | Baja      |
| Module order    | Listado de tikets con filtros avanzados                      | Alta      |
| Module user     | El administrador puede gestionar los user                    | Alta      |
| Module user     | Envío de Emails en el registro y recuperación de contraseñas | Media     |
| Dashboard       | CRUD de order, user y operator                               | Media     |
| Module user     | user deben poder registrarse e iniciar sesión                | Alta      |

---

# 🧱 Sprint Backlog

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
- [ ] Dashboard de administrador (gestión de user, order, etc.)

### Herramientas sugeridas:

- Figma (para diseño y prototipado)
- Notion / Trello / Jira (para vincular tareas con diseños)

---

# 🧱 **Sprint 1** 🏃‍♂️ Backend & Frontend

- **Fecha de Inicio:** 13/enero/2025
- **Fecha de Finalización:** 13/febrero/2025
- **Duración del Sprint:** 4 semanas
- **Objetivo del Sprint:** Finalizar la gestión de user, operator y completar el panel de administración básico.

### ✅ Historias de Usuario y Tareas

| Historia/Tarea          | Descripción                                                             | Estado      |
| :---------------------- | :---------------------------------------------------------------------- | :---------- |
| Gestión de user         | Crear, editar, eliminar y listar user desde el panel de administración. | En progreso |
| Gestión de operator     | Crear, editar, eliminar y listar operator.                              | En progreso |
| Panel de Administración | Implementar CRUD de órdenes, user y operator.                           | En progreso |

### 🎯 Entregables

- CRUD de user funcionando.
- CRUD de operator funcionando.
- Sección inicial del panel administrativo operativa.

---

# 🧱 **Sprint 2** 🏃‍♂️ Mobile

---

# 🧱 **Sprint 3** 🏃‍♂️ Pruebas y Optimización

---

# 🧱 **Sprint 4** 🏃‍♂️ Entrega Final y Capacitación

---

# 🧱 **Sprint Extra** 🏃‍♂️ Patient Module

## 📦 **Product Backlog**

| Función/Tarea | Descripción                                    | Prioridad |
| ------------- | ---------------------------------------------- | --------- |
| Patient       | Subir documentos del paciente y/o acompañantes | Alta      |
| Patient       | Vista publica de carga de documentos           | Alta      |
| Patient       | Descargar PDF con los documentos               | Media     |

---

- **Fecha de Inicio:** 30/abril/2025
- **Fecha de Finalización:** 06/mayo/2025
- **Duración del Sprint:** 1 semana
- **Objetivo del Sprint:** Gestión de documentos del paciente

### ✅ Historias de Usuario y Tareas

| Historia/Tarea | Descripción                                                             | Estado      |
| :------------- | :---------------------------------------------------------------------- | :---------- |
| Database       | Crear, editar, eliminar y listar user desde el panel de administración. | En progreso |

### 🎯 Entregables

- Subir documentos del paciente y/o acompañantes
- Visualizar documentos del paciente
- Borrar documentos del paciente
- ***
