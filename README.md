# Creativa Studio — versión web

Aplicación web adaptable a móviles. Puede publicarse como sitio estático; no necesita servidor propio ni base de datos para las funciones incluidas.

## Funciones actuales
- Foto y color: brillo, contraste, saturación, escala de grises, rotación y exportación PNG.
- Dibujo táctil: color, tamaño de pincel, borrador y exportación PNG.
- Vídeo y audio: seleccionar y reproducir archivos compatibles.
- PDF y archivos de texto: lectura y vista previa según el navegador.
- Animación: demostración interactiva.

## Probar
Para que funcionen bien los módulos y la instalación como aplicación web, publícala en un alojamiento HTTPS estático. No es necesario ejecutar una compilación para esta versión: los archivos HTML, CSS y JavaScript se sirven directamente.

## Publicar gratis con GitHub Pages desde el celular
1. Crea una cuenta o inicia sesión en https://github.com.
2. Crea un repositorio nuevo, por ejemplo `creativa-studio`.
3. Sube todos los archivos y carpetas de este ZIP a la raíz del repositorio. Deben quedar `index.html`, `src/`, `manifest.webmanifest`, `icon.svg` y `.github/workflows/` en la raíz.
4. Abre la pestaña **Actions** y habilita GitHub Actions si te lo solicita.
5. En **Settings → Pages**, selecciona **GitHub Actions** como método de publicación.
6. La acción **Deploy Creativa Studio Web** publicará el sitio cuando subas cambios a la rama `main`. Si el repositorio usa otra rama, cambia `main` en el archivo `.github/workflows/deploy-web.yml`.
7. Cuando la acción termine en verde, abre la URL de GitHub Pages que aparece en Settings → Pages.
8. En Android, abre esa URL en Chrome y usa el menú ⋮ → **Añadir a pantalla de inicio**. La opción de instalación como PWA depende del navegador y del alojamiento HTTPS.

## Privacidad y límites
Esta versión no carga las imágenes, audio, vídeo ni documentos a un servidor desde el código incluido; los archivos seleccionados se procesan en el navegador. No es una suite profesional equivalente a Adobe. Audio y vídeo son reproductores, PDF se visualiza según soporte del navegador y la animación es una demostración. Evita abrir archivos sensibles en dispositivos compartidos.
