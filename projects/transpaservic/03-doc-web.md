<!-- guion.md -->
<!-- Escena -->

# Intro

¡Bienvenidos a `TranspaServic`, la solución definitiva para la gestión de órdenes y ticketes de transporte de pasajeros!  
Hoy te guiaremos por las principales funcionalidades de la plataforma para que puedas sacarle el máximo provecho.

---

### PANTALLA PRINCIPAL

- Inicio de sesión
- Recuperar contraseña
- App de TranspaServic
- Consultar por documento

Comencemos con el `inicio de sesión`. Ingresa tu correo y contraseña para acceder a tu cuenta.

¿Olvidaste tu contraseña? No te preocupes, haz clic en `Recuperar contraseña` y sigue los pasos para restablecerla rápidamente.

---

### PANORAMA GENERAL DE LA PLATAFORMA

- Gestion de Ordenes
- Gestion de Usuarios
- Gestion de Operadores
- Perfil y Respaldo de Base de Datos
- Modo Claro y Oscuro

Desde el `menú lateral`, como administrador, puedes gestionar `órdenes, usuarios y operadores`, además de configurar tu perfil y realizar copias de seguridad de la base de datos.

Vamos a explorar estas opciones.

Sabemos que la comodidad visual es clave. `TranspaServic` ofrece `modo claro y oscuro` para adaptarse a tus preferencias.

---

### GESTION DE ÓRDENES Y TICKETES

- Lista de órdenes con barra de búsqueda y filtros

  En la sección de `órdenes`, puedes `consultar, crear, editar y eliminar` registros. La barra de búsqueda permite encontrar órdenes por `cliente, itinerario, operador o estado`. Además, los filtros avanzados te ayudan a organizar la información por `rango de fechas y estado de la orden`.

- Opcion para elegir número de órdenes paginadas

  Puedes ajustar la cantidad de órdenes por página según tus necesidades.

- Exportación de datos

Necesitas reportes detallados? `TranspaServic` te permite exportar la información en formato `Excel o PDF`, ya sea de una orden específica o de una selección filtrada. el PDF es ideal para imprimir.

### Detalle de la órden

Si deseas ver el detalle completo de una orden, haz clic en una orden y se te abrirá una nueva ventana con la información de la orden.

- Información de la orden
- busqueda por numero de orden \*
- boton para editar la orden (presionar)
- exportar orden en formato PDF listo para imprimir
- Historial de la orden

#### Aprobación de la orden

- Fecha real de viaje
- Numero de Ticket
- Cantidad usada (se limita a la cantidad emitida)
- Eliminar order (solo administrador)

  Al completar una orden, es importante registrar la fecha, los datos del cliente y `adjuntar una foto del ticket` para confirmar el servicio.

#### Registro de la orden

- No Contrato y No de Orden son unicos en cada orden
- Tipo de documento
- Codigo de pais: digite 57 para Colombia
- Telefono para enviar mensajes a whatsapp
- Habilitar el envio de recordatorios por whatsapp
- Notificaciones por web y movil al finalizar el registro

¿Vas a crear una orden? Registra los datos de la operadora, el usuario, fechas, origen y destino. Una vez guardada, puedes enviar un recordatorio automático por WhatsApp para asegurar la notificación.

#### Importación de datos

- Seleccionar archivo con datos duplicados
- Mostrar datos duplicados en pantalla

  ¿Ya tienes una base de datos en el formato excel? `Impórtala` y `TranspaServic` la listará automáticamente para que la consultes y edites fácilmente.

- Habilitar/deshabilitar el envio de recordatorios por whatsapp

  Envía `recordatorios por WhatsApp y correo electrónico` a operadores y usuarios con un solo clic. Gracias a la conexión con la API de WhatsApp, también puedes consultar el estado de los mensajes en la sección de `reportes`.

#### Notificaciones

- Los operadores recibirán Notificaciones cuando se genere una nueva orden o se importen datos.

---

# GESTION DE USUARIOS

- Lista de usuarios con barra de búsqueda y filtros

  Desde la sección de `usuarios`, puedes `crear, revisar, editar y eliminar` registros. Utiliza la barra de búsqueda y los filtros para encontrar rápidamente la información que necesitas.

- Gestion de usuarios, crear, editar, eliminar y ver detalles de un usuario

#### Registro de usuario

Para agregar un usuario, solo completa su `nombre, correo electrónico y número de WhatsApp`. Puedes `generar una contraseña aleatoria` y consultar su valor en cualquier momento.

- Selección de rol

  Define el rol del usuario: ¿Será `usuario, administrador o colaborador`? Asigna el perfil adecuado según su función dentro del sistema.

  - `usuario`: Acceso limitado a funciones de un operador.
  - `administrador`: Acceso completo a todas las funciones.
  - `colaborador`: Acceso a funciones de administración con limitaciones a la base de datos.

- Habilitar/deshabilitar el envio de email con la contraseña aleatoria

---

# GESTION DE OPERADORES

- Lista de operadores

  El proceso para `operadores` funciona de la misma manera que para los usuarios. Registra la información de la línea de transporte y asigna los datos de contacto necesarios.

---

# RESPALDO DE BASE DE DATOS

- crear, restaurar y eliminar respaldo de base de datos
- respaldo diario automatico, manteniendo backup de 7 ultimos dias.
- carga y descarga de respaldo de base de datos

  Si eres administrador, cuentas con un `respaldo diario` de la base de datos. Cada copia se mantiene por `7 días`, eliminándose automáticamente al octavo día.

# PERFIL

Desde `tu perfil`, puedes `consultar y editar` tu información personal.

---

# DESPEDIDA

- Logo de TranspaServic con efecto de salida
- Logo de Systered: `Desarrollado por Systered`

TranspaServic está diseñado para hacer que la gestión de Ticketes de pasajeros sea simple, eficiente y automatizada.

¡Explora todas sus funcionalidades y lleva tu operación al siguiente nivel!

¡Gracias por acompañarnos en este recorrido! Nos vemos en el próximo video.
