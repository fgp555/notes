Volver al [inicio](../)

# 🗓️ Scrum - Sistema de Turnos Médicos

## 🧾 Información General

- **Usuarios principales:** Doctores (profesionales)
- **Tipo de turnos:** Citas médicas
- **Reservas:** Solo de forma interna
- **Datos de cada turno:** Nombre del paciente, fecha, hora, tipo de servicio, profesional asignado
- **Roles de usuario:** Admin y Profesional
- **Canal de notificación:** WhatsApp
- **Frontend & Backend:** Monorepo con ReactJS + NestJS + PostgreSQL
- **Despliegue:** Todo en cPanel
- **Deadline MVP:** 1 mes

---

## 🧱 Entidades Clave

- **Patient**
- **Turn**
- **Service**
- **Professional** (con atributo `isAdmin`)

---

## 🔗 Relaciones Principales

- `Professional` puede ofrecer muchos `Services`
- `Turn` está relacionado con:
  - un `Patient`
  - un `Professional`
  - un `Service`

---

## 📌 Vistas necesarias (Frontend)

- Login
- Reservar turno (formulario)
- Mis turnos
- Panel de administración

---

## 🧩 Funcionalidades Clave

- Login con email
- Gestión de turnos
- Gestión de usuarios
- Historial de turnos
- Notificación por WhatsApp
- Reprogramación y cancelación
- Disponibilidad por profesional y servicio
- Límite de 8 horas diarias por profesional

---

## 🧑‍💻 Sprints

### 🚀 Sprint 1 (Semana 1): Autenticación y Modelo de Datos

#### Historias de Usuario

- Como **profesional**, quiero iniciar sesión con mi correo.
- Como **admin**, quiero registrar nuevos profesionales.

#### Tareas

- [ ] Crear entidades: Patient, Turn, Service, Professional
- [ ] Autenticación con JWT (NestJS)
- [ ] Registro y login (React)
- [ ] Gestión de roles (admin, profesional)

---

### 📅 Sprint 2 (Semana 2): Gestión de Turnos

#### Historias de Usuario

- Como **profesional**, quiero agregar turnos disponibles según mis servicios.
- Como **admin**, quiero ver todos los turnos y filtrarlos.

#### Tareas

- [ ] CRUD de turnos (NestJS)
- [ ] Formulario de reserva de turno (React)
- [ ] Validaciones de disponibilidad por servicio y profesional
- [ ] Restricción de 8 horas por día

---

### 📊 Sprint 3 (Semana 3): Panel y Funciones Adicionales

#### Historias de Usuario

- Como **profesional**, quiero ver mis turnos agendados.
- Como **admin**, quiero poder cancelar o reprogramar turnos.

#### Tareas

- [ ] Vista de "Mis turnos"
- [ ] Funcionalidad de cancelar y reprogramar
- [ ] Historial de turnos por paciente y profesional
- [ ] Panel administrativo para ver todo

---

### 📣 Sprint 4 (Semana 4): Notificaciones y Deploy

#### Historias de Usuario

- Como **profesional**, quiero que el paciente reciba confirmación por WhatsApp.

#### Tareas

- [ ] Integración con WhatsApp API (ej: Twilio o Wati.io)
- [ ] Tests básicos de flujo de turnos
- [ ] Deploy full stack en cPanel (React y NestJS)

---

## ✅ Prioridad MVP

> Funcionalidad crítica: **Agregar turno**

---

¿Querés que también prepare el modelo de base de datos con relaciones (diagramado o en SQL/NestJS)? También puedo ayudarte con los endpoints REST y estructura del backend si querés ir armando los módulos.
