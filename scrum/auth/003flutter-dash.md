# 📌 Historia Auth-003 – Dashboard y rutas privadas con roles (Flutter)

**Como** usuario autenticado,  
**quiero** acceder a un dashboard con contenido según mi rol,  
**para que** vea opciones según si soy administrador o usuario común, y mantener mi sesión activa.

---

## ✅ Criterios de Aceptación

- [ ] Si no estoy autenticado, se me redirige automáticamente a la vista de login.
- [ ] Si estoy autenticado, se me redirige automáticamente a `/dashboard`.
- [ ] Si tengo el rol `admin`:
  - [ ] Se muestra una lista de usuarios.
  - [ ] Cada usuario tiene un botón para eliminarlo.
  - [ ] Se realiza una petición DELETE al backend al eliminar.
- [ ] Si tengo el rol `user`:
  - [ ] Solo se muestra información de mi perfil (nombre, correo, etc.).
- [ ] Al actualizar la página, la sesión debe mantenerse activa.
- [ ] Se utiliza el token guardado (en `SharedPreferences` o `SecureStorage`) para validar la sesión.
- [ ] Las rutas privadas están protegidas desde el frontend.

---

## 📘 Definition of Done (DoD)

- [ ] Rama `feature/dashboard-auth-routing` creada.
- [ ] Se utilizó `Navigator` o `GoRouter` para proteger rutas privadas.
- [ ] Se implementó lógica para redireccionar según login y rol.
- [ ] El token JWT se valida y se reutiliza al refrescar.
- [ ] Se implementó vista de administrador con eliminación de usuarios.
- [ ] Se implementó vista de usuario con perfil visible.
- [ ] La eliminación de usuarios se hace con petición DELETE y encabezado Authorization.
- [ ] El diseño es accesible y se probó en diferentes tamaños de pantalla.

---

## ⏱️ Estimación

> 3–4 días

---

## 📎 Referencias

- [Flutter navigation](https://docs.flutter.dev/ui/navigation)
- [Flutter dio](https://pub.dev/packages/dio)
- [Flutter Secure Storage](https://pub.dev/packages/flutter_secure_storage)

---

## 🌐 Backend

**Repositorio:**  
https://github.com/fgp555/express-js-login.git

**Despliegue:**  
https://express-js-login.onrender.com/

---

## 🔐 Requests

**GET – Lista de Usuarios (solo admin)**
```
GET https://express-js-login.onrender.com/api/users
Authorization: Bearer mocked.token.123456
Content-Type: application/json
```

**DELETE – Eliminar Usuario (por ID)**
```
DELETE https://express-js-login.onrender.com/api/users/1
Authorization: Bearer mocked.token.123456
Content-Type: application/json
```

---

## 📌 Preguntas Técnicas

- ¿Cómo almacenar y restaurar el token de sesión al recargar la app?
- ¿Cuál es la mejor forma de proteger rutas según roles en Flutter?
- ¿Cómo manejar errores si se intenta acceder a recursos restringidos?
