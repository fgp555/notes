# 📌 Historia Auth-001 – Registro de usuario (Flutter)

**Como** nuevo visitante,  
**quiero** registrarme en el sistema con mi nombre, correo y contraseña,  
**para que** pueda crear una cuenta y acceder a funcionalidades privadas.

---

## ✅ Criterios de Aceptación

- [ ] El formulario de registro tiene los campos: `name`, `email`, `password`, y opcionalmente `confirmPassword`.
- [ ] Todos los campos visibles son obligatorios y se validan antes de enviar:
  - [ ] El campo `email` debe tener un formato válido (`TextFormField` con `validator`).
  - [ ] El campo `password` debe tener al menos 6 caracteres.
  - [ ] Si `confirmPassword` está presente, debe coincidir con `password`.
- [ ] Cada campo valida en tiempo real o al perder el foco (`onChanged` o `onFieldSubmitted`).
- [ ] Al enviar el formulario:
  - [ ] Se desactiva el botón y se muestra un `CircularProgressIndicator`.
  - [ ] Se realiza una petición `POST` usando `http.post` o `Dio`.
- [ ] Si el registro es exitoso:
  - [ ] Se navega automáticamente a la pantalla de login.
- [ ] Si ocurre un error (por ejemplo, email ya registrado), se muestra un mensaje en un `SnackBar` o `AlertDialog`.
- [ ] Los campos de contraseña permiten mostrar/ocultar su contenido con un ícono (👁️):
  - [ ] Si el formulario **no incluye `confirmPassword`**, el campo `password` debe tener un ícono para mostrar/ocultar la contraseña.
  - [ ] Si el formulario **incluye `confirmPassword`**, ambos campos deben tener íconos de mostrar/ocultar contraseña.

---

## 📘 Definition of Done (DoD)

- [ ] Rama `feature/register-flutter` creada.
- [ ] Se utilizó el paquete `http` o `dio` para conectarse con el backend.
- [ ] Se implementó validación local (`Form` + `TextFormField`).
- [ ] Se implementó el estado de carga y error usando `setState`, `Provider`, `Bloc`, etc.
- [ ] El diseño es responsivo y accesible (usabilidad móvil, contraste, campos accesibles).
- [ ] La pantalla fue probada en dispositivos físicos y/o emuladores (Android/iOS).

---

## ⏱️ Estimación

> libre

---

## 📎 Referencias

- [flutter.dev - Forms](https://docs.flutter.dev/cookbook/forms/validation)  
- [Dio (HTTP Client)](https://pub.dev/packages/dio)  
- [Provider](https://pub.dev/packages/provider)  
- [FormBuilder](https://pub.dev/packages/flutter_form_builder)

---

## 🔐 Request de prueba

```http
POST http://localhost:3000/api/auth/register
Content-Type: application/json

{
  "name": "Juan Pérez",
  "email": "juan@example.com",
  "password": "123456"
}
```

---

## 📌 Tools

- [mini-postman](https://frank-gp.github.io/app/mini-postman/)

---

## 📌 Preguntas Frecuentes

- ¿Cuál es el riesgo de no validar la coincidencia entre `password` y `confirmPassword` antes de enviar?
- ¿Qué experiencia es mejor: mostrar los errores en tiempo real o al enviar?

---

## 📌 Buenas prácticas a debatir

- ¿Conviene usar `SnackBar`, `Dialog`, o indicadores visuales por campo para mostrar errores?
- ¿Es mejor validar en el backend si el correo ya existe y notificar claramente, o solo devolver un error genérico?