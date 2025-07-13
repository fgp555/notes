# 📌 Historia Auth-003 – Dashboard y rutas privadas con roles (Next.js)

**Como** usuario autenticado,  
**quiero** acceder a un dashboard con contenido según mi rol,  
**para que** vea opciones específicas si soy admin o usuario común, y mantener mi sesión activa incluso al actualizar.

---

## ✅ Criterios de Aceptación

- [ ] Si no estoy autenticado, se me redirige automáticamente a la ruta `/login`.
- [ ] Si estoy autenticado, se me redirige automáticamente a `/dashboard`.
- [ ] Si tengo el rol `admin`:
  - [ ] Se muestra una tabla o lista con todos los usuarios.
  - [ ] Cada usuario tiene un botón para eliminarlo.
  - [ ] Al eliminar un usuario se envía una petición DELETE con el token JWT en los headers.
- [ ] Si tengo el rol `user`:
  - [ ] Se muestra solo su información de perfil.
- [ ] Al actualizar el navegador, la sesión se mantiene activa si hay token guardado.
- [ ] Las rutas privadas están protegidas en el lado cliente (y opcionalmente en SSR).
- [ ] Crear una instancia de `axios` con el token JWT en el cliente.

---

## 📘 Definition of Done (DoD)

- [ ] Rama `feature/dashboard-auth-nextjs` creada.
- [ ] Se implementó protección de rutas con `getServerSideProps` o `middleware` si es necesario.
- [ ] Se usó `axios` para comunicar con el backend.
- [ ] Se validó y restauró el token desde cookies o localStorage.
- [ ] Se usó Context API o una librería como `next-auth`, `react-query` o `zustand` para estado de sesión. (opcional)
- [ ] El dashboard se adapta al rol y muestra la información correspondiente.

---

## ⏱️ Estimación

> libre

---

## 📎 Referencias

- [Next.js Middleware](https://nextjs.org/docs/middleware)
- [next-auth](https://next-auth.js.org/)
- [react-query](https://tanstack.com/query/latest)
- [axios](https://axios-http.com/)
- [Next.js App Router Auth Example](https://github.com/vercel/examples/tree/main/auth/js)

---

## 🌐 Backend

**Repositorio:**  
https://github.com/fgp555/express-js-login.git

**Despliegue:**  
https://express-js-login.onrender.com/

---

## 🔐 Requests

**GET – Lista de Usuarios (solo admin)**

```sh
GET https://express-js-login.onrender.com/api/users
Authorization: Bearer mocked.token.123456
Content-Type: application/json
```

**DELETE – Eliminar Usuario (por ID)**

```sh
DELETE https://express-js-login.onrender.com/api/users/1
Authorization: Bearer mocked.token.123456
Content-Type: application/json
```

---

## 📌 Preguntas Técnicas

- ¿Dónde es mejor almacenar el token en Next.js: `localStorage`, `cookie` o `sessionStorage`?
- ¿Cómo hacer que las rutas estén protegidas desde SSR en lugar de solo en el cliente?
- ¿Qué patrón de manejo de sesión es más escalable en Next.js?
