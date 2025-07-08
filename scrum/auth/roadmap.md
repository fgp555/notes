# 🛣️ Roadmap de Historias de Usuario – Autenticación (Auth)

Este roadmap contempla la implementación modular del sistema de autenticación (Auth) para un proyecto web con manejo de sesiones, roles y seguridad.

---

## 🔐 Autenticación y Registro Básico

### 🧾 Historia 001 – Registro de usuarios

**Como** visitante,  
**quiero** poder registrarme con mi nombre, correo y contraseña,  
**para que** pueda acceder a funcionalidades privadas.

---

### 🧾 Historia 002 – Inicio de sesión

**Como** usuario registrado,  
**quiero** poder iniciar sesión con mis credenciales,  
**para que** acceda a mi cuenta.

---

### 🧾 Historia 003 – Validación de formularios (Frontend + Backend)

**Como** usuario,  
**quiero** recibir mensajes de error si ingreso datos inválidos,  
**para que** pueda corregirlos fácilmente.

---

## 🧾 Manejo de Sesiones

### 🧾 Historia 004 – Generación y almacenamiento de token (JWT)

**Como** usuario autenticado,  
**quiero** que se genere un token al iniciar sesión,  
**para que** se mantenga mi sesión activa en el frontend.

---

### 🧾 Historia 005 – Protección de rutas privadas

**Como** visitante,  
**quiero** ser redirigido al login si intento acceder a páginas privadas,  
**para que** no acceda sin estar autenticado.

---

## 👮 Roles y Permisos

### 🧾 Historia 006 – Asignación de roles (admin, cliente, mesero, etc.)

**Como** administrador,  
**quiero** asignar un rol a cada usuario,  
**para que** cada uno vea solo lo que le corresponde.

---

### 🧾 Historia 007 – Restricción de vistas según el rol

**Como** usuario con rol limitado,  
**quiero** acceder solo a las páginas correspondientes a mi rol,  
**para que** no vea funcionalidades que no debo usar.

---

## 🔄 Recuperación y Seguridad

### 🧾 Historia 008 – Recuperar contraseña (vía email o token)

**Como** usuario,  
**quiero** poder restablecer mi contraseña si la olvido,  
**para que** pueda recuperar el acceso.

---

### 🧾 Historia 009 – Cierre de sesión (logout)

**Como** usuario,  
**quiero** poder cerrar sesión de forma segura,  
**para que** nadie más acceda a mi cuenta en ese dispositivo.

---

## 🛡️ Seguridad Extra

### 🧾 Historia 010 – Prevención de ataques (rate limit, captcha, etc.)

**Como** desarrollador,  
**quiero** proteger el login y registro con medidas de seguridad,  
**para que** se eviten ataques automáticos o de fuerza bruta.

---

## 📅 Orden sugerido por sprints

| Sprint | Historias sugeridas                   |
| ------ | ------------------------------------- |
| 01     | 001 – Registro de usuarios            |
|        | 002 – Inicio de sesión                |
|        | 003 – Validación de formularios       |
| 02     | 004 – Generación de token             |
|        | 005 – Protección de rutas             |
|        | 006 – Asignación de roles             |
| 03     | 007 – Restricción por rol             |
|        | 008 – Recuperar contraseña            |
|        | 009 – Logout                          |
| 04     | 010 – Seguridad (rate limit, captcha) |
|        | QA Final, testing de flujo completo   |
