# 📌 Historia Front-004 – Refresh Token

**Como** usuario autenticado,  
**quiero** mantener mi sesión activa mediante tokens de acceso y refresh,  
**para que** no se me cierre la sesión automáticamente tras expirar el token.

---

## ✅ Criterios de Aceptación

- [ ] Al expirar el token de acceso (accessToken), se intenta renovar automáticamente con un `refreshToken`.
- [ ] El `refreshToken` se almacena en una cookie o localStorage.
- [ ] El frontend detecta que el token ha expirado (ej. 401) y solicita un nuevo accessToken usando el refreshToken.
- [ ] Si el refreshToken es válido, se recibe un nuevo accessToken y se actualiza el estado global.
- [ ] Si el refreshToken falla (caducado o inválido), se redirige al login y se borra el estado de sesión.
- [ ] Las peticiones protegidas se reintentan automáticamente después de refrescar el token.
- [ ] Si el accessToken o refreshToken no existen o son inválidos, se guarda la URL actual en localStorage para redirigir al iniciar sesión nuevamente. (modificar el login para redirigir a la URL anterior)

---

## 🧩 Implementation Notes

- [ ] Se crea una instancia personalizada de `axios` con un interceptor para manejar expiraciones.
- [ ] El interceptor detecta el error `401 Unauthorized`, hace el refresh y reintenta la petición original.
- [ ] Se debe evitar múltiples llamadas de refresh simultáneas (ej. usando una cola o bandera de estado).
- [ ] La sesión se mantiene activa mientras el refreshToken sea válido.
- [ ] Antes de redirigir al login, se guarda la URL actual (window.location.href) en localStorage con una clave como redirectAfterLogin.

---

## 🛠️ Definition of Done (DoD)

- [ ] Se implementa un sistema de refresh token en el backend y frontend.
- [ ] Se usa `axios` con interceptores para renovar tokens automáticamente.
- [ ] El refreshToken se almacena de forma segura en cookies o localStorage.
- [ ] La sesión del usuario es persistente sin necesidad de volver a iniciar sesión frecuentemente.
- [ ] En caso de error con el refreshToken, se limpia el estado global y se redirige al login.

---

# Request

```sh
@ACCESS_TOKEN_ADMIN={{$dotenv ACCESS_TOKEN_ADMIN}}
@ACCESS_TOKEN_USER={{$dotenv ACCESS_TOKEN_USER}}
@REFRESH_TOKEN={{$dotenv REFRESH_TOKEN}}

### decodeToken solo para desarrollo
POST http://localhost:3000/api/auth/decode-token
Authorization: Bearer {{ACCESS_TOKEN_ADMIN}}

### refreshToken
POST http://localhost:3000/api/auth/refresh-token
Authorization: Bearer {{REFRESH_TOKEN}}
```
