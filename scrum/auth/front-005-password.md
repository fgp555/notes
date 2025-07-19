# 📌 Historia Auth-005 – Recuperar contraseña (Frontend)

**Como** usuario que olvidó su contraseña,  
**quiero** solicitar un enlace de restablecimiento por correo y establecer una nueva contraseña,  
**para que** pueda volver a acceder a mi cuenta.

---

## ✅ Criterios de Aceptación

### 📨 Solicitud de Restablecimiento

- [ ] El formulario tiene un único campo: `email`.
- [ ] El campo `email` es obligatorio y debe tener formato válido.
- [ ] Al enviar el formulario:
  - [ ] Se muestra un loader/spinner y se desactiva el botón.
  - [ ] Se realiza `POST` a `/api/auth/forgot-password` con el `email` y el `baseURL`.
  - [ ] Se muestra un mensaje genérico de éxito, como: "Si el correo está registrado, recibirás un enlace para restablecer tu contraseña".
  - [ ] Si ocurre un error de red/servidor, se muestra un mensaje claro al usuario.

### 🔑 Restablecimiento de Contraseña

- [ ] El usuario llega al formulario de nueva contraseña desde un enlace que incluye un `resetToken`.
- [ ] El formulario tiene los campos:
  - `newPassword`
  - `confirmPassword`
- [ ] Ambos campos son obligatorios.
  - [ ] `newPassword` debe tener al menos 6 caracteres.
  - [ ] `confirmPassword` debe coincidir con `newPassword`.
- [ ] Al enviar el formulario:
  - [ ] Se desactiva el botón y se muestra loader.
  - [ ] Se realiza `POST` a `/api/auth/restore-password` con el `resetToken` y la nueva contraseña.
  - [ ] Si es exitoso:
    - [ ] Se muestra un mensaje como: "Contraseña restablecida con éxito".
    - [ ] Se redirige al login.
  - [ ] Si el token es inválido o expiró, se muestra un error claro al usuario.

---

## 📘 Definition of Done (DoD)

- [ ] Rama `feature/password` creada.
- [ ] Formulario de solicitud de email conectado al backend con `axios`.
- [ ] Formulario de nueva contraseña que toma `resetToken` desde la URL.
- [ ] Validaciones por campo (`onBlur`) y al enviar.
- [ ] Muestra feedback de errores y éxito.
- [ ] Componentes accesibles, responsive y con UX amigable.
- [ ] Flujo probado en navegador (desktop y móvil).

---

## ⏱️ Estimación

> libre

---

## 📎 Referencias

- [axios](https://axios-http.com/)
- [Token Reset con JWT – Seguridad](https://owasp.org/www-project-cheat-sheets/cheatsheets/Forgot_Password_Cheat_Sheet.html)

---

# 📌 Tools

- [mini-postman](https://frank-gp.github.io/app/mini-postman/)

---

## 🔐 Requests de prueba

### 📨 Enviar enlace de restablecimiento

---

```sh
###
POST http://localhost:3000/api/auth/forgot-password
Content-Type: application/json

{
  "email": "fgp555@gmail.com",
  "baseURL": "http://localhost:3000"
}

###
POST http://localhost:3000/api/auth/restore-password
Content-Type: application/json

{
  "resetToken": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImZncDU1NUBnbWFpbC5jb20iLCJ1c2VySWQiOiI2ODdhZjQ5M2E2ZmQzOGE5NDM3OWJjYjIiLCJ0b2tlblR5cGUiOiJyZXNldCIsImlhdCI6MTc1Mjg4OTQ2MywiZXhwIjoxNzUyODg5NzYzfQ.5X0LdlkZ6SoyRPIZXV1wqPVbe_5ShEsO_XCzaf8MmnM",
  "newPassword": "newSecurePass456"
}

```

---

## 📌 Preguntas Frecuentes

- ¿Dónde debe almacenarse temporalmente el token? ¿En query params (`?token=...`) o en localStorage?
- ¿Qué mensaje es más claro para el usuario tras restablecer la contraseña: “Redirigido al login” o “Contraseña cambiada, ahora puedes iniciar sesión”?
