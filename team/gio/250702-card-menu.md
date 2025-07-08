# 📌 Historia de Usuario

**Como** comensal de restaurante y/o mesero,  
**quiero** ver el menú en formato grid con cards completas,  
**para que** pueda visualizar la lista de menús y acceder al detalle de cada uno de forma rápida y clara.

---

## ✅ Criterios de Aceptación

- [ ] El usuario puede ver los menús como tarjetas (`cards`) distribuidas en una cuadrícula (`grid`).
- [ ] Cada tarjeta muestra al menos: nombre del menú, imagen y precio.
- [ ] Al hacer clic en una tarjeta, esta se expande o abre una vista detalle.
- [ ] En la vista detalle se muestra: nombre del menú, descripción, precio.
- [ ] En el modo detalle se puede navegar al siguiente menú sin cerrar el modal o card expandida (tipo navegación vertical).
- [ ] El componente debe integrar íconos desde FontAwesome CDN (ya habilitado en el proyecto).

---

## 🏷️ Prioridad

> Media

## ⏱️ Estimación

> 3–5 días

## 👤 Asignado a

> Giovanna MR

---

## 📎 Referencias

- [Diseño en Figma - Menu Cards](https://www.figma.com/design/Sb4JnG1Z37KdffD4VsCv6b/restufy?node-id=28-6&t=xnSmfvl6FEWz9IJQ-1)
- [FontAwesome Icons](https://fontawesome.com/search)

---

## 📚 Referencias de aprendizaje

- [Navegación vertical inspirada - Codepen](https://codepen.io/hrtzt/pen/pgXMYb)

# Git

```sh
# Crea y cambia a una nueva rama basada en la rama 'main' remota
git checkout -b card-menu origin/main

# Pushear
git add .
git commit -m 'comentario'
git push -u origin card-menu
```
