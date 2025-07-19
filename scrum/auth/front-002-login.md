# 📌 Historia Auth-002 – Inicio de sesión (Frontend)

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
- [ ] Usar un estado global para gestionar la sesión del usuario.
- [ ] El estado global de autenticación se actualiza con los datos del usuario y token.
- [ ] Al iniciar sesión exitosamente, se redirige al dashboard u otra vista protegida.
- [ ] Si la respuesta es un error, se muestra un mensaje claro.

---

## 📘 Definition of Done (DoD)

- [ ] Rama `feature/login-frontend` creada.
- [ ] Se usó `axios` o `fetch` para comunicarse con el backend.
- [ ] Se incluyó manejo de estado de carga y errores.
- [ ] El token fue almacenado correctamente y se usa en headers al navegar.
- [ ] Se implementó redirección condicional después del login.
- [ ] Se creó y utilizó un estado global (`AuthContext`, `Zustand`, `Redux`, etc.) para gestionar la sesión del usuario.
- [ ] Otros componentes del sistema pueden acceder al estado de autenticación sin necesidad de props.

---

## ⏱️ Estimación

> libre

---

## 📎 Referencias

- [axios](https://axios-http.com/)

---

# 📌 Tools

- [mini-postman](https://frank-gp.github.io/app/mini-postman/)

---

### Requests

```sh
### user
POST http://localhost:3000/api/auth/login
Content-Type: application/json

{
    "email": "user@gmail.com",
    "password": "user@gmail.com"
}

### admin
POST http://localhost:3000/api/auth/login
Content-Type: application/json

{
    "email": "admin@gmail.com",
    "password": "admin@gmail.com"
}
```

# 📌 Preguntas Frecuentes

> - 👉 ¿Cuándo deberíamos usar una ruta relativa (`/api/auth/login`) y cuándo una absoluta (`https://domain.com/auth/login`)? Explica los pros, contras y contexto.
> - ¿Qué riesgos podrían existir al dejar rutas absolutas hardcodeadas en el código cliente?
> - ¿Cuando usar `npm run dev` y cuando usar `npm start`?

# 📌 Ejemplo de buena práctica a debatir:

> - ¿Considerarían buena práctica crear un archivo src/config/apiRoutes.js que contenga todas las rutas del backend y usarlas desde ahí? ¿Por qué sí o por qué no?
