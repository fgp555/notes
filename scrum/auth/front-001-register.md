# 📌 Historia Auth-001 – Registro de usuario (Frontend)

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
- [ ] Al hacer blur (perder el foco) en cada campo, se validan y muestran errores si corresponde.
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
- [ ] El formulario implementa validación por campo con eventos `onBlur`.
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

# 📌 Tools

- [mini-postman](https://frank-gp.github.io/app/mini-postman/)

---

## 🔐 Requests de prueba

**Petición Local**

```
POST http://localhost:3000/api/auth/register
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
- ¿Qué feedback es más útil para el usuario: mostrar errores al enviar o al salir de cada campo?

---

## 📌 Buenas prácticas a debatir

- ¿Es buena práctica mostrar errores específicos por campo (`email ya está en uso`) o errores genéricos (`verifica tus datos`)?
