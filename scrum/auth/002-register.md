# 📌 Historia Auth-002 – Registro de usuarios

**Como** visitante del sitio,  
**quiero** poder registrarme con mi nombre, correo electrónico y contraseña,  
**para que** pueda crear una cuenta y acceder a funciones exclusivas del sistema.

---

## ✅ Criterios de Aceptación

- [ ] El formulario de registro debe estar disponible públicamente.
- [ ] El formulario incluye los campos:
  - `name` (input texto requerido)
  - `email` (input tipo email, requerido y único)
  - `password` (input tipo password, mínimo 6 caracteres)
  - `confirmPassword` (debe coincidir con `password`)
- [ ] Todos los campos requeridos deben validarse en frontend y backend.
- [ ] Si el email ya está registrado, debe mostrar un mensaje claro al usuario.
- [ ] Al enviar datos válidos:
  - Se debe crear el usuario en la base de datos.
  - Se debe enviar una respuesta JSON con éxito.
- [ ] Al finalizar el registro, se puede:
  - [ ] Redirigir al login
  - [ ] O iniciar sesión automáticamente (dependiendo del flujo definido)
- [ ] El botón de registro debe deshabilitarse durante el envío (para evitar doble submit).
- [ ] El formulario debe mostrar mensajes de error específicos por campo.

---

## 📘 Definition of Done (DoD)

- [ ] Se creó la rama `feature/register`.
- [ ] Se implementó el endpoint `POST /api/auth/register` en Express.js.
- [ ] El backend valida los campos y almacena el nuevo usuario con contraseña encriptada (ej: bcrypt).
- [ ] Se usa una librería de validación (como `express-validator`) en el backend.
- [ ] El frontend implementa el formulario con validaciones de campos.
- [ ] Se realizó manejo de errores y mensajes amigables para el usuario.
- [ ] El código fue revisado por al menos un miembro del equipo.
- [ ] La funcionalidad fue probada correctamente en desktop y móvil.

---

## ⏱️ Estimación

> 2 días

---

## 📎 Referencias

- [bcrypt – Encriptación de contraseñas en Node.js](https://www.npmjs.com/package/bcrypt)
- [express-validator – Validación de formularios](https://express-validator.github.io/docs/)
- [Figma o mockup del formulario (si aplica)](#)

---

## 📚 Referencias de aprendizaje

- [Form validation with React Hook Form](https://react-hook-form.com/)
- [Best Practices for User Registration Forms – UX](https://uxdesign.cc/design-better-forms-96fadca0f49c)
- [Node.js Registration with JWT (tutorial)](https://www.digitalocean.com/community/tutorials/nodejs-jwt-expressjs)
