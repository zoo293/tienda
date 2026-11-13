# GAMEVERSE – librerías integradas

Se añadieron dos librerías ligeras al proyecto existente, sin cambiar la estructura de sus páginas ni reemplazar el CSS original.

## 1. SweetAlert2
- Uso: reemplaza los avisos básicos del navegador por ventanas más claras para avisar cuando un producto ya está en el carrito, cuando se intenta pagar con el carrito vacío y para mostrar mensajes de compra.
- Archivo integrado: `abrir1ro.html` carga SweetAlert2 antes de `app.js`; `app.js` usa la función `gvAviso()`.
- Documentación: https://sweetalert2.github.io/

## 2. AOS (Animate On Scroll)
- Uso: agrega animaciones suaves a las tarjetas de videojuegos cuando aparecen al desplazarse por el catálogo.
- Archivo integrado: `abrir1ro.html` carga AOS y `app.js` configura las tarjetas automáticamente.
- Documentación: https://michalsnik.github.io/aos/

## Cómo ejecutar
1. Extrae el ZIP completo.
2. Abre la carpeta en Visual Studio Code.
3. Abre `index.html` con Live Server (recomendado).
4. Inicia sesión o crea una cuenta y entra al catálogo.

## Importante
Las dos librerías se cargan desde CDN, por lo que se necesita conexión a internet para ver sus efectos. Si SweetAlert2 no carga, los avisos usan automáticamente `alert()` como respaldo. El login y el carrito siguen siendo demostrativos y guardan información en `localStorage`; no constituyen un sistema de autenticación ni pagos de producción.
