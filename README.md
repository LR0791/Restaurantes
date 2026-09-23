# Mis Restaurantes

App personal para llevar el control de tus restaurantes favoritos, reservas y visitas. Funciona como una app instalable en iPhone/iPad (PWA), sin necesidad de subirla a la App Store.

## Contenido del proyecto

```
index.html                      → la app completa (HTML + CSS + JS en un solo fichero)
manifest.json                    → configuración de la app instalable (nombre, colores, iconos)
icons/
  icon-192.png                    → icono 192x192 (Android/manifest)
  icon-512.png                    → icono 512x512 (Android/manifest, pantalla de carga)
  apple-touch-icon.png             → icono 180x180 (iPhone y iPad estándar)
  apple-touch-icon-120.png         → icono 120x120 (iPhone más antiguos)
  apple-touch-icon-152.png         → icono 152x152 (iPad)
  apple-touch-icon-167.png         → icono 167x167 (iPad Pro)
  favicon-32.png                   → icono pequeño para la pestaña de Safari
```

Se incluyen varios tamaños del mismo icono para que se vea nítido en cualquier iPhone o iPad, sin recortes ni pixelado.

---

## Paso 1 — Subir el proyecto a GitHub

1. Entra en [github.com](https://github.com) e inicia sesión (o crea una cuenta gratuita).
2. Pulsa el botón **"+"** de arriba a la derecha → **"New repository"**.
3. Ponle un nombre, por ejemplo `mis-restaurantes`. Debe ser **público** para que GitHub Pages sea gratis.
4. Pulsa **"Create repository"**.
5. En la página del repositorio, pulsa **"uploading an existing file"** (o **"Add file" → "Upload files"**).
6. Arrastra dentro **todo el contenido** de esta carpeta descomprimida: el fichero `index.html`, `manifest.json`, y la carpeta `icons` completa con sus 7 imágenes. Asegúrate de que `icons` se sube como carpeta, no que las imágenes queden sueltas en la raíz.
7. Escribe un mensaje como "Primera versión" y pulsa **"Commit changes"**.

## Paso 2 — Activar GitHub Pages

1. Dentro del repositorio, ve a **"Settings"**.
2. En el menú de la izquierda, pulsa **"Pages"**.
3. En **"Branch"**, selecciona `main` y la carpeta `/ (root)`. Pulsa **"Save"**.
4. Espera 1-2 minutos. GitHub te dará una URL parecida a:
   `https://tu-usuario.github.io/mis-restaurantes/`
5. Esa es la dirección de tu app. Guárdala.

## Paso 3 — Instalar en iPhone / iPad

1. Abre **Safari** (tiene que ser Safari) en el iPhone o iPad.
2. Ve a la URL del Paso 2.
3. Pulsa el icono **⬆️ Compartir**.
4. Baja hasta **"Añadir a pantalla de inicio"** y pulsa.
5. Verás una vista previa del icono (el plato, tenedor y cuchillo) — así se verá en tu pantalla de inicio. Pulsa **"Añadir"** arriba a la derecha.

El icono se verá nítido y completo, sin bordes raros, tanto en iPhone como en iPad. Al abrir la app funcionará a pantalla completa, sin la barra de Safari.

Repite el Paso 3 en cada dispositivo donde quieras instalarla — es la misma URL para todos.

## Actualizar la app en el futuro

Cuando tengas una nueva versión de `index.html`:
1. Entra en el repositorio de GitHub.
2. Abre el fichero `index.html` → pulsa el lápiz (✏️ Edit) → pega el contenido nuevo → "Commit changes".
   *(O bien "Add file → Upload files" y sube el nuevo `index.html`, sobrescribiendo el anterior.)*
3. Los cambios tardan uno o dos minutos en aparecer en GitHub Pages.
4. En el iPhone/iPad no hace falta reinstalar nada: la próxima vez que abras la app, Safari cargará la versión nueva (puede que tengas que cerrarla del todo y reabrirla una vez).

Si en algún momento cambias el icono, sustituye los ficheros dentro de `icons/` manteniendo los mismos nombres, y no hará falta tocar nada más.

## Notas

- Los datos de tus restaurantes se guardan **en el propio dispositivo** (localStorage), no en GitHub. Cada iPhone/iPad tiene su propia lista independiente salvo que uses **Exportar JSON / Importar JSON** desde "Acerca de" para pasar los datos de un dispositivo a otro, o la opción de **compartir restaurantes por WhatsApp** (🔗 en la lista principal).
