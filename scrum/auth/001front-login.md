# 📌 Historia Auth-001 – Inicio de sesión (Frontend)

**Como** usuario registrado,  
**quiero** iniciar sesión desde el frontend con mi correo y contraseña,  
**para que** pueda acceder a mi cuenta protegida en el sistema.

---

## ✅ Criterios de Aceptación

- [ ] El formulario de login tiene campos `email` y `password`.
- [ ] Ambos campos se validan antes de enviar (no vacíos, email válido).
- [ ] Al enviar, se muestra un loader/spinner y se desactiva el botón.
- [ ] Se realiza la petición POST al backend con las credenciales.
- [ ] Si la respuesta incluye un token, se almacena en `localStorage` o cookie segura.
- [ ] Al iniciar sesión exitosamente, se redirige al dashboard u otra vista protegida.
- [ ] Si la respuesta es un error, se muestra un mensaje claro.

---

## 📘 Definition of Done (DoD)

- [ ] Rama `feature/login-frontend` creada.
- [ ] Se usó `axios` o `fetch` para comunicarse con el backend.
- [ ] Se incluyó manejo de estado de carga y errores.
- [ ] El token fue almacenado correctamente y se usa en headers al navegar.
- [ ] Se implementó redirección condicional después del login.

---

## ⏱️ Estimación

> libre

---

## 📎 Referencias

- [axios](https://axios-http.com/)
<!-- - [Diseño de formulario en Figma (si aplica)](#) -->

# Recursos

### Backend Repositorio

- [https://github.com/fgp555/express-js-login.git](https://github.com/fgp555/express-js-login.git)

### Backend Despliegue

- [https://express-js-login.onrender.com](https://express-js-login.onrender.com/)
