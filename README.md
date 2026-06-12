# Mis Gastos

Aplicación web progresiva (PWA) para llevar el control de gastos personales desde el móvil o el ordenador. Funciona sin conexión, sin cuenta y sin servidor: los datos se guardan únicamente en tu dispositivo.

## Características

- Registro rápido de gastos repartidos en 17 categorías (fijas y variables).
- Resumen mensual con gráfico de tarta y desglose por categoría.
- Lectura automática de tickets, capturas de la app del banco y PDF de extractos: extrae los movimientos y los clasifica.
- Pegado de movimientos desde el chat del banco, con pantalla de revisión antes de guardar y aviso de posibles duplicados.
- Exportación de copia de seguridad en CSV.
- Instalable como app en el móvil y con un diseño adaptado también a pantalla de ordenador.

## Tecnología

- Un único archivo `index.html` con todo el HTML, CSS y JavaScript, sin frameworks ni dependencias externas.
- Almacenamiento local en el navegador (`localStorage`).
- Service worker (`sw.js`) para el funcionamiento sin conexión.
- Clasificación de movimientos asistida por la API de Anthropic (Claude).

## Archivos del proyecto

- `index.html` — toda la aplicación.
- `manifest.json` — configuración de la PWA (nombre, iconos, colores).
- `sw.js` — service worker para la caché y el modo sin conexión.
- `icon-192.png`, `icon-512.png` — iconos de la app.

## Cómo desplegar

El proyecto se publica con GitHub Pages. Para actualizarlo:

1. Edita los archivos y haz commit a la rama `main`.
2. GitHub Pages publica los cambios automáticamente en uno o dos minutos.

## Privacidad

Todos los gastos se guardan solo en el dispositivo, en el almacenamiento local del navegador. No hay servidor ni base de datos externa, así que conviene exportar una copia en CSV de vez en cuando como respaldo.
