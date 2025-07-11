# 📌 Historia Auth-002 – Registro de usuario (Frontend)

**Como** nuevo visitante,  
**quiero** registrarme en el sistema con mi nombre, correo y contraseña,  
**para que** pueda crear una cuenta y acceder a funcionalidades privadas.

---

## ✅ Criterios de Aceptación

- [ ] El formulario de registro tiene los campos: `name`, `email`, `password`, `confirmPassword`.
- [ ] Todos los campos son obligatorios y se validan antes de enviar.
  - [ ] El campo `email` debe tener formato válido.
  - [ ] `password` debe tener mínimo 6 caracteres.
  - [ ] `confirmPassword` debe coincidir con `password`.
- [ ] Al enviar, se muestra un loader/spinner y se desactiva el botón.
- [ ] Se realiza la petición `POST` al backend con los datos del formulario.
- [ ] Si el registro es exitoso:
  - [ ] Se redirige al login.
- [ ] Si ocurre un error (por ejemplo, email ya registrado), se muestra un mensaje claro.

---

## 📘 Definition of Done (DoD)

- [ ] Rama `feature/register-frontend` creada.
- [ ] Se usó `axios` para enviar datos al backend.
- [ ] Se incluyó manejo de estado de carga (`loading`) y errores (`errorMessage`).
- [ ] El código tiene validaciones en cliente antes de enviar datos.
- [ ] El componente es accesible y responsive.
- [ ] El flujo fue probado en navegador (desktop y móvil).

---

## ⏱️ Estimación

> libre

---

## 📎 Referencias

- [axios](https://axios-http.com/)

---

## 🌐 Recursos

**Repositorio Backend:**  
https://github.com/fgp555/express-js-login.git

**Despliegue Backend:**  
https://express-js-login.onrender.com/

---

## 🔐 Requests de prueba

**Peticion Local**

```
POST http://localhost:3000/api/auth/register
Content-Type: application/json

{
  "name": "Juan Pérez",
  "email": "juan@example.com",
  "password": "123456"
}
```

**Peticion Remota**

```
POST https://express-js-login.onrender.com/api/auth/register
Content-Type: application/json

{
  "name": "Juan Pérez",
  "email": "juan@example.com",
  "password": "123456"
}
```

---

## 📌 Preguntas Frecuentes

- ¿Cuál es el riesgo de no validar la coincidencia entre `password` y `confirmPassword` antes de enviar?

---

## 📌 Buenas prácticas a debatir

- ¿Es buena práctica mostrar errores específicos por campo (`email ya está en uso`) o errores genéricos (`verifica tus datos`)?
