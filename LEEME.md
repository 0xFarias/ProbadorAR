# Probador AR — demo

Página de prueba de realidad aumentada web con `<model-viewer>` 4.3.1.

## Contenido

- `index.html` — la página.
- `modelos/refrigeradora.glb` — 70 × 180 × 74 cm.
- `modelos/televisor-55.glb` — 123 × 71 × 3 cm (se coloca en la pared).
- `modelos/lampara-de-pie.glb` — 44 × 165 × 44 cm.
- `modelos/sofa.glb` — 219 × 79 × 102 cm. «Glam Velvet Sofa» © 2021 Wayfair, LLC, licencia CC BY 4.0, de Khronos glTF Sample Assets.

## Publicarla en GitHub Pages (para probar la cámara AR en el celular)

1. Crea un repositorio público en GitHub, por ejemplo `probador-ar`.
2. Sube `index.html` y la carpeta `modelos` tal como están (Add file → Upload files).
3. En el repositorio entra a Settings → Pages, en «Branch» elige `main` y la carpeta `/ (root)`, y guarda.
4. Espera uno o dos minutos y abre `https://TU-USUARIO.github.io/probador-ar/` en el celular.
5. Toca «Ver en mi espacio».

Desde la computadora, la misma página muestra un código QR para abrirla en el celular.

## Requisitos para que se abra la cámara

- La página debe abrirse con HTTPS (GitHub Pages ya lo da).
- Android: Chrome y la app «Servicios de Google Play para RA» (ARCore).
- iPhone: Safari. El archivo USDZ para AR Quick Look se genera solo a partir del GLB.

## Para pasarla a tu tienda

Cambia la lista `PRODUCTOS` al inicio del script de `index.html` (nombre, categoría, ruta del `.glb`, `lugar`: `floor` o `wall`) o genérala desde tu base de datos. Cada modelo debe estar en metros y a tamaño real.
