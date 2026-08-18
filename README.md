# Sitio personal — Luis Fernando Escobar Caba

Sitio construido con **Jekyll**, el motor que usa GitHub Pages de forma nativa
(no necesitás instalar nada ni programar: GitHub lo construye automáticamente
cada vez que hacés `push`).

## Cómo publicarlo (una sola vez)

1. En GitHub, creá un repositorio **público** llamado exactamente:
   `Lufesc.github.io`
   (el nombre debe ser igual a tu usuario + `.github.io`, así GitHub sabe que es tu sitio personal)
2. Subí todo el contenido de esta carpeta a la raíz de ese repositorio
   (podés arrastrar los archivos desde la web de GitHub, o usar git desde tu compu).
3. Andá a **Settings → Pages** del repo y confirmá que la fuente sea
   `Deploy from a branch` → rama `main` → carpeta `/ (root)`.
4. En 1-2 minutos tu sitio va a estar en:
   **https://lufesc.github.io**

## Cómo editarlo después

Todo el contenido está en archivos `.md` (Markdown), fáciles de editar
directamente desde GitHub (botón del lápiz ✏️ en cada archivo):

- `index.md` → página de inicio (Sobre mí)
- `cv.md` → tu CV
- `docencia.md` → tarjetas que enlazan a tus cursos (cada curso es OTRO repo,
  ver más abajo)
- `investigacion.md` → publicaciones y working papers

Cada vez que guardás un cambio ("Commit changes") en GitHub, el sitio se
actualiza solo en 1-2 minutos. No hace falta instalar Jekyll ni ningún programa.

## Agregar tu CV en PDF

Subí tu PDF a `assets/cv-luis-escobar.pdf` (mismo nombre) y el botón de
"Descargar CV" en `cv.md` va a funcionar automáticamente.

## Estructura

```
index.md              → home
cv.md                  → CV
docencia.md            → cursos (enlaza a repos de curso)
investigacion.md       → publicaciones
_config.yml            → título, datos de contacto, configuración del sitio
_layouts/default.html  → plantilla visual (no hace falta tocarla)
assets/css/style.css   → estilos (colores, tipografía)
assets/img/photo.png   → tu foto
```

## Conectar tus cursos

Cada materia que dictás puede vivir en su propio repositorio, igual que
`docencia.md` ya enlaza a `https://lufesc.github.io/econometria/`.
Repetí el mismo patrón (ver el repo `econometria` incluido) para
Estadística Aplicada, Modelación Financiera, etc. — copiá esa carpeta,
cambiá el contenido y creá un nuevo repo por materia.
