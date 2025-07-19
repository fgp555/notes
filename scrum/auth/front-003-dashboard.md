# 📌 Historia Auth-003 – Dashboard y rutas privadas con roles (Next.js)

**Como** usuario autenticado,  
**quiero** acceder a un dashboard con contenido según mi rol,  
**para que** vea opciones específicas si soy admin o usuario común, y mantener mi sesión activa incluso al actualizar.

---

## ✅ Criterios de Aceptación

- [ ] Si no estoy autenticado, se me redirige automáticamente a la ruta `/login`.
- [ ] Si estoy autenticado, se me redirige automáticamente a `/dashboard`.
- [ ] Al actualizar el navegador, la sesión se mantiene activa si hay token guardado (en `localStorage` o cookie).
- [ ] Las rutas privadas están protegidas en el lado cliente (con `useRouter`) y opcionalmente desde SSR (`getServerSideProps` o `middleware`).
- [ ] Crear una instancia de `axios` que incluya automáticamente el token JWT en los headers.

### 👤 Rol: `user`

- [ ] Se muestra solo su información de perfil (nombre, email, rol).
- [ ] Puede editar su propia información.
- [ ] Se envía una petición `PATCH` al backend con el token JWT:

### 🛠️ Rol: `admin`

- [ ] Se muestra una tabla o lista con todos los usuarios.
- [ ] Cada usuario tiene:
  - [ ] Botón para eliminar usuario (`DELETE /api/users/remove/:id`).
  - [ ] Botón para editar usuario (abre formulario de edición y envía `PATCH`).
  - [ ] Se incluye su propio perfil (admin) en la lista o vista separada.

---

## 📘 Definition of Done (DoD)

- [ ] Rama `feature/dashboard` creada.
- [ ] Se implementó protección de rutas con `getServerSideProps` o `middleware` si es necesario.
- [ ] Se usó `axios` para comunicar con el backend.
- [ ] Se creó una instancia de `axios` con manejo automático del token JWT.
- [ ] Se validó y restauró el token desde cookies o `localStorage`.
- [ ] Se usó Context API o una librería como `next-auth`, `react-query`, `zustand` o `Redux Toolkit` para el manejo de sesión y usuario.
- [ ] El dashboard se adapta al rol y muestra la información correspondiente.
- [ ] Se implementó funcionalidad para actualizar los datos de usuario (perfil y/o desde el panel admin).
- [ ] Se manejaron correctamente los estados de carga y error al editar y eliminar usuarios.
- [ ] Se integró Redux Toolkit con slices para `auth` y `users`, incluyendo `thunks` asincrónicos para login, carga de perfil, edición y eliminación de usuarios.

---

## ⏱️ Estimación

> libre

---

## 📎 Referencias

- [Redux Toolkit](https://redux-toolkit.js.org/)
- [Next.js Middleware](https://nextjs.org/docs/14/app/building-your-application/routing/middleware)
- [axios](https://axios-http.com/)

---

## 🔐 Requests

```sh
@ACCESS_TOKEN_ADMIN={{$dotenv ACCESS_TOKEN_ADMIN}}
@ACCESS_TOKEN_USER={{$dotenv ACCESS_TOKEN_USER}}

###
GET http://localhost:3000/api/users/findAll
Authorization: Bearer {{ACCESS_TOKEN_ADMIN}}

###
GET http://localhost:3000/api/users/findOne/687aedc7a9b9dce563b1d35e
Authorization: Bearer {{ACCESS_TOKEN_USER}}

### Update user
PATCH http://localhost:3000/api/users/update/687aedc7a9b9dce563b1d35e
Authorization: Bearer {{ACCESS_TOKEN_ADMIN}}
Content-Type: application/json

{
    "name": "ana_admin",
    "email": "ana_admin@gmail.com",
    "password": "ana_admin@gmail.com",
    "role": "admin"
}

###
DELETE http://localhost:3000/api/users/remove/687aa8f2874a04aed3183f62
Authorization: Bearer {{ACCESS_TOKEN_ADMIN}}
```

---

## 📌 Preguntas Técnicas

- ¿Dónde es mejor almacenar el token en Next.js: `localStorage`, `cookie` o `sessionStorage`?
- ¿Cómo hacer que las rutas estén protegidas desde SSR en lugar de solo en el cliente?
- ¿Qué patrón de manejo de sesión es más escalable en Next.js?
