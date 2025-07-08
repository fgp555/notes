# 📌 Historia Auth-001 – Inicio de sesión

**Como** usuario registrado,  
**quiero** poder iniciar sesión con mis credenciales,  
**para que** acceda a mi cuenta.

---

## ✅ Criterios de Aceptación

- [ ] El usuario puede iniciar sesión proporcionando su correo electrónico y contraseña.
- [ ] Si las credenciales son correctas, se debe generar un token (JWT) en el backend.
- [ ] El token debe ser enviado al frontend en la respuesta.
- [ ] El frontend debe almacenar el token de forma segura (por ejemplo, en `localStorage` o `HttpOnly Cookie`, según se defina).
- [ ] Si las credenciales son incorrectas, se debe mostrar un mensaje claro al usuario.
- [ ] El formulario debe validar que el email y la contraseña no estén vacíos.
- [ ] Al iniciar sesión exitosamente, debe redirigirse al dashboard o vista protegida.
- [ ] El formulario debe mostrar un indicador de carga (spinner o similar) durante la petición.
- [ ] Debe evitarse múltiples envíos con un botón deshabilitado temporalmente.

---

## 📘 Definition of Done (DoD)

- [ ] Se creó la rama `feature/login`.
- [ ] Se implementó el endpoint `/api/auth/login` en el backend con Express.js.
- [ ] El backend valida credenciales y genera un token JWT válido.
- [ ] El frontend envía los datos correctamente usando `fetch` o `axios`.
- [ ] El formulario tiene validaciones básicas y muestra mensajes de error.
- [ ] El token recibido es almacenado y se utiliza para futuras peticiones autenticadas.
- [ ] El código fue revisado por al menos 1 miembro del equipo.
- [ ] La funcionalidad fue probada en staging o local.
- [ ] Se realizaron pruebas manuales en móvil y escritorio.

---

## ⏱️ Estimación

> 2 días

---

## 📎 Referencias

- [Diseño de formulario en Figma (si aplica)](#)
- [Login con JWT – JWT.io](https://jwt.io/)
- [Flow básico de login con token – Auth0 Blog](https://auth0.com/blog/)

---

## 📚 Referencias de aprendizaje

- [express.json() – Middleware para parseo de cuerpo](https://expressjs.com/en/api.html#express.json)
- [jsonwebtoken – Librería JWT para Node.js](https://github.com/auth0/node-jsonwebtoken)
- [axios – Librería para HTTP requests](https://axios-http.com/)
- [Validación de formularios con React Hook Form](https://react-hook-form.com/)
