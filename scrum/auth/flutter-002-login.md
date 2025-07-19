# 📌 Historia Auth-001 – Inicio de sesión (Flutter)

**Como** usuario registrado,  
**quiero** iniciar sesión desde una aplicación Flutter con mi correo y contraseña,  
**para que** pueda acceder a mi cuenta protegida en el sistema.

---

## ✅ Criterios de Aceptación

- [ ] El formulario de login tiene campos `email` y `password`.
- [ ] Ambos campos se validan antes de enviar (no vacíos, email con formato válido).
- [ ] Al enviar, se muestra un loader/spinner y se desactiva el botón de envío.
- [ ] Se realiza la petición POST al backend usando `http` o `dio`.
- [ ] Si la respuesta incluye un token, se almacena en `SharedPreferences` o `SecureStorage`.
- [ ] Al iniciar sesión exitosamente, se navega a una vista protegida (como un dashboard).
- [ ] Si ocurre un error, se muestra un mensaje claro en pantalla.
- [ ] Se evita el envío duplicado mientras se está cargando.

---

## 📘 Definition of Done (DoD)

- [ ] Rama `feature/login-flutter` creada.
- [ ] Se utilizó `http` o `dio` para enviar la solicitud al backend.
- [ ] Se incluyó manejo de estado de carga y errores.
- [ ] El token fue almacenado correctamente en `SharedPreferences` o `FlutterSecureStorage`.
- [ ] Se implementó navegación condicional luego del login exitoso.
- [ ] Se realizaron pruebas en Android y iOS (si aplica).
- [ ] El diseño es responsivo y accesible.

---

## ⏱️ Estimación

> libre

---

## 📎 Referencias

- [Flutter http](https://pub.dev/packages/http)
- [Flutter dio](https://pub.dev/packages/dio)
- [Flutter Secure Storage](https://pub.dev/packages/flutter_secure_storage)
- [Flutter Form Validation](https://flutter.dev/docs/cookbook/forms/validation)

---

## 🌐 Backend

**Repositorio:**  
https://github.com/fgp555/express-js-login.git

**Despliegue:**  
https://express-js-login.onrender.com/

---

## 🔐 Requests de prueba

**Login Local**
```
POST http://localhost:3000/api/auth/login
Content-Type: application/json

{
  "email": "admin@example.com",
  "password": "123456"
}
```

**Login Remoto**
```
POST https://express-js-login.onrender.com/api/auth/login
Content-Type: application/json

{
  "email": "admin@example.com",
  "password": "123456"
}
```

---

## 📌 Preguntas Técnicas

- ¿Cuál es la mejor forma de manejar tokens de forma segura en Flutter?
- ¿Deben mostrarse mensajes genéricos o específicos si el login falla?
- ¿Cómo evitar múltiples peticiones si el usuario presiona varias veces el botón?

---

## 📌 Buenas prácticas a debatir

- ¿Es recomendable separar las rutas de API en un archivo como `api_constants.dart`?
- ¿Se debería usar un `provider`, `bloc`, `riverpod` u otro patrón para manejar el estado de autenticación?
