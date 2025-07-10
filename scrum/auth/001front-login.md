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

# Requests

```sh
### 🔐 LOGIN Local
POST http://localhost:3000/api/auth/login
Content-Type: application/json

{
  "email": "admin@example.com",
  "password": "123456"
}
```

```sh
### 🔐 LOGIN Remoto
POST https://express-js-login.onrender.com/api/auth/login
Content-Type: application/json

{
  "email": "admin@example.com",
  "password": "123456"
}
```

# 📌 Preguntas Frecuentes

> - 👉 ¿Cuándo deberíamos usar una ruta relativa (`/api/auth/login`) y cuándo una absoluta (`https://domain.com/auth/login`)? Explica los pros, contras y contexto.

> - ¿Qué riesgos podrían existir al dejar rutas absolutas hardcodeadas en el código cliente?

> - ¿Cuando usar `npm run dev` y cuando usar `npm start`?

# 📌 Ejemplo de buena práctica a debatir:

> - ¿Considerarían buena práctica crear un archivo src/config/apiRoutes.js que contenga todas las rutas del backend y usarlas desde ahí? ¿Por qué sí o por qué no?
