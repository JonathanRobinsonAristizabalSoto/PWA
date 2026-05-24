# Mi Primera PWA

## Descripción
Una Progressive Web App (PWA) sencilla y didáctica que muestra cómo registrar un Service Worker, cachear recursos y permitir la instalación en la pantalla de inicio.

## Qué hace (resumen)
- Cachea archivos para que la app funcione sin conexión.
- Muestra un modal propio (centrado) para iniciar la instalación.
- Llama al diálogo nativo del navegador para completar la instalación.

## Estructura de archivos
- `index.html` — Página principal y modales.
- `app.js` — Registro del Service Worker, manejo de `beforeinstallprompt` y modales.
- `service-worker.js` — Lógica de caché (install / activate / fetch).
- `manifest.json` — Metadatos de la PWA (nombre, iconos, start_url).
- `styles.css` — Estilos y reglas para centrar los modales.
- `img/icons/` — Iconos usados por el `manifest.json` (añadir PNGs si faltan).

## Requisitos
- Navegador moderno con soporte PWA (Chrome, Edge, Firefox).
- Servir desde `localhost` o HTTPS (los Service Workers requieren origen seguro).
- (Opcional) Python o Node.js para levantar un servidor local.

## Ejecutar localmente (Windows — PowerShell)
Con Python:
```powershell
python -m http.server 8000