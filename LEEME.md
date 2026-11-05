# curiositapp en GitHub Pages (con logo y sin conexión)

## Qué contiene
- `index.html`: la app completa (1.700+ curiosidades, 3 idiomas, estadísticas)
- `manifest.webmanifest`: nombre, colores e iconos
- `sw.js`: guarda todo en el móvil para usarlo sin conexión
- `icons/`: logo en 192, 512, maskable y apple-touch (180)

## Subirlo a GitHub (desde el navegador, sin instalar nada)
1. Entra en github.com, inicia sesión y pulsa **New repository**.
2. Nombre: `curiositapp`. Público. Marca "Add a README" y pulsa **Create repository**.
3. En el repositorio: **Add file > Upload files**. Arrastra el CONTENIDO de la carpeta
   (index.html, manifest.webmanifest, sw.js y la carpeta icons). Pulsa **Commit changes**.
   (Si subes el .zip, descomprímelo antes: GitHub no lo descomprime.)
4. **Settings > Pages**. En "Build and deployment" elige *Deploy from a branch*,
   rama `main`, carpeta `/ (root)`, y **Save**.
5. Espera 1-2 minutos. Tu app estará en: `https://TU-USUARIO.github.io/curiositapp/`

## Instalarla en el iPhone
1. Abre esa dirección en **Safari** (tiene que ser Safari).
2. Pulsa el botón Compartir y luego **Añadir a pantalla de inicio**.
3. Ábrela una vez con internet y deja que cargue. Desde entonces funciona sin conexión,
   a pantalla completa y con su logo.

## Actualizar la app
Sustituye `index.html` en GitHub y cambia en `sw.js` la línea `const VERSION = "v1";`
por `"v2"` (luego `"v3"`...). Así los móviles descargan la versión nueva al abrir con internet.

## Nota
Las estadísticas se guardan en el propio iPhone. Si borras los datos de Safari o
la app de la pantalla de inicio, se pierden.
