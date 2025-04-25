Volver al [inicio](../)

# 🎓 Scrum - Plataforma Educativa para Emprendedores

## 🧾 Información General

- **Objetivo:** Informar, capacitar, inspirar y crear comunidad.
- **Audiencia:** Emprendedores nuevos, en crecimiento, segmentados por sector o país.
- **Tipo de contenido:** Cápsulas en video, artículos, reseñas, texto, audio e infografías.
- **Modelo:** Curso estructurado con progresión por módulos.
- **Tecnologías:** NestJS, ReactJS, PostgreSQL, cPanel
- **Freemium:** Algunos módulos gratuitos, otros de pago.
- **Deadline MVP:** 1 mes

---

## 👥 Roles de Usuario

- **Estudiante**
- **Mentor**
- **Administrador**

---

## 🔗 Funcionalidades del MVP

### 👤 Autenticación y Usuarios

- Registro e inicio de sesión con email.
- Perfil de usuario con progreso.
- Marcar contenido como visto o favorito.
- Visualizar estadísticas de avance personal.
- Módulo freemium (acceso limitado sin pago).

### 🎥 Gestión y Consumo de Contenido

- Subir cápsulas desde el panel admin.
- Crear módulos y agrupar contenido educativo.
- Contenido embebido desde YouTube.
- Visualización de texto, imágenes y video.
- Estructura del curso por progresión (orden secuencial).
- Evaluaciones y quizzes al final de cada módulo.
- Sistema de certificación al finalizar rutas completas.

### 💬 Comunidad e Interacción

- Comentarios por cápsula o módulo.
- Recomendaciones de películas, series y análisis de empresarios.
- Artículos y cápsulas actualizadas por autores colaboradores.

---

## 🧱 Entidades Clave (Base de Datos)

- **User** (id, name, email, role, progress, etc.)
- **Module** (id, title, description, order)
- **Capsule** (id, title, type [video/text/quiz], content_url, module_id, is_free)
- **Progress** (user_id, capsule_id, completed_at)
- **Quiz** (id, capsule_id, question, options, correct_answer)
- **Favorite** (user_id, capsule_id)
- **Comment** (user_id, capsule_id, content, created_at)

---

## 📌 Rutas/Vistas (Frontend)

- Home / Landing
- Registro / Login
- Dashboard estudiante (módulos, progreso, favoritos)
- Página de módulo con cápsulas
- Visualizador de cápsulas
- Quiz al finalizar cápsulas
- Panel de administrador (gestión de cápsulas y módulos)

---

## 🧑‍💻 Sprints

### 🎨 Sprint 0 (Semana 0): Diseño UI/UX y estructura visual

#### Objetivo:

Tener todos los diseños listos en Figma para comenzar a desarrollar con una guía visual clara y consistente.

#### Entregables:

- Sistema visual (tipografía, colores, botones, espaciado, iconografía).
- Prototipos de vistas principales (desktop y mobile).
- Documentación de componentes UI reutilizables.
- Flujo de navegación y experiencia de usuario.
- Link de Figma compartido con el equipo.

#### Vistas a diseñar:

- [ ] Landing page / Home
- [ ] Registro e inicio de sesión
- [ ] Dashboard de estudiante (progreso, módulos, favoritos)
- [ ] Visualización de cápsula (video, texto, infografía, quiz)
- [ ] Evaluación tipo quiz
- [ ] Certificado
- [ ] Panel admin (gestión de cápsulas y módulos)
- [ ] Vista de mentor (opcional)

#### Herramientas sugeridas:

- Figma (para diseño y prototipado)
- Notion / Trello / Jira (para vincular tareas con diseños)

---

### 🚀 Sprint 1 (Semana 1): Base del sistema y usuarios

#### Historias de Usuario

- Como **estudiante**, quiero registrarme para acceder al contenido gratuito.
- Como **admin**, quiero poder crear módulos y cápsulas educativas.

#### Tareas

- [ ] Estructura del proyecto (NestJS + React + DB)
- [ ] Registro/Login con JWT
- [ ] Gestión de usuarios con roles
- [ ] CRUD básico de módulos y cápsulas
- [ ] Frontend: registro/login + navegación base

---

### 📚 Sprint 2 (Semana 2): Consumo de contenido

#### Historias de Usuario

- Como **estudiante**, quiero acceder a las cápsulas en orden para aprender paso a paso.
- Como **admin**, quiero subir cápsulas embebidas desde YouTube.

#### Tareas

- [ ] Embebido de videos de YouTube
- [ ] Vistas de módulos y cápsulas
- [ ] Marcar cápsulas como vistas
- [ ] Guardar como favorito
- [ ] Avance por usuario
- [ ] Frontend de vista de cápsula

---

### 🧠 Sprint 3 (Semana 3): Quizzes y comunidad

#### Historias de Usuario

- Como **estudiante**, quiero responder quizzes para evaluar mi aprendizaje.
- Como **usuario**, quiero comentar en cápsulas y módulos.

#### Tareas

- [ ] Sistema de quizzes por cápsula
- [ ] Guardar resultados del quiz
- [ ] Sistema de comentarios
- [ ] Visualización de respuestas y feedback
- [ ] Panel admin para subir quizzes

---

### 🏁 Sprint 4 (Semana 4): Certificación y deploy

#### Historias de Usuario

- Como **estudiante**, quiero recibir un certificado al finalizar un módulo.
- Como **admin**, quiero monitorear el avance de los usuarios.

#### Tareas

- [ ] Generación de certificados (PDF/HTML)
- [ ] Panel de seguimiento por usuario
- [ ] Estadísticas básicas (vistas, progreso, quizzes)
- [ ] Tests básicos y QA
- [ ] Deploy completo en cPanel

---

## ✅ Prioridades MVP

> Funcionalidades clave del MVP:

- [x] Registro/login
- [x] Subir y mostrar cápsulas
- [x] Acceso a módulos estructurados
- [x] Marcar cápsulas como vistas
- [x] Reproducción de contenido embebido
