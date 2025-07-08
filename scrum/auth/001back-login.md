# 📌 Historia Auth-001 – Inicio de sesión (Backend)

**Como** desarrollador backend,  
**quiero** implementar un endpoint seguro para iniciar sesión,  
**para que** los usuarios puedan autenticarse y obtener un token válido (JWT).

---

## ✅ Criterios de Aceptación

- [ ] Se implementó el endpoint `POST /api/auth/login`.
- [ ] El backend valida el email y la contraseña recibida.
- [ ] Si las credenciales son válidas, se genera un token JWT.
- [ ] Si las credenciales son incorrectas, se retorna error con mensaje claro.
- [ ] El JWT incluye información mínima: userId, role, y expiración.
- [ ] La contraseña se compara usando `bcrypt`.
- [ ] El sistema retorna el token en la respuesta JSON.

---

## 📘 Definition of Done (DoD)

- [ ] Rama `feature/login-backend` creada.
- [ ] Se validaron los datos de entrada con `express-validator` u otra librería.
- [ ] Se usó `jsonwebtoken` para generar el token.
- [ ] La contraseña se validó usando `bcrypt.compare`.
- [ ] Se agregaron respuestas de error estructuradas.
- [ ] Se protegieron posibles errores con `try/catch`.
- [ ] El código fue revisado por al menos 1 miembro del equipo.
- [ ] El endpoint fue probado con Postman y cubierto por pruebas básicas.

---

## ⏱️ Estimación

> 1 día

---

## 📎 Referencias

- [bcrypt](https://www.npmjs.com/package/bcrypt)
- [jsonwebtoken](https://github.com/auth0/node-jsonwebtoken)
- [express-validator](https://express-validator.github.io/docs/)
