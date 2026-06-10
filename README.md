# Ramon Rueda — Portfolio (Neon Retro)

Portafolio de Data Science con estética synthwave/neón retro. Un solo archivo
(`index.html`) sin dependencias ni build — listo para GitHub Pages.

## Cómo publicarlo en https://rayrcol.github.io/

```bash
# 1. Clona tu repo de GitHub Pages (si no lo tienes local)
git clone https://github.com/RayRCol/rayrcol.github.io.git
cd rayrcol.github.io

# 2. Reemplaza el index.html con el nuevo
cp ~/Desktop/MIT/rayrcol-portfolio/index.html .

# 3. Sube los cambios
git add index.html
git commit -m "Rediseño neon retro del portafolio"
git push
```

En 1–2 minutos GitHub Pages actualiza el sitio.

## Para verlo en local

```bash
python3 -m http.server 4173 --directory ~/Desktop/MIT/rayrcol-portfolio
# abre http://localhost:4173
```

## Personalización rápida

- **Colores**: variables CSS al inicio del `<style>` (`--cyan`, `--magenta`, `--purple`, `--yellow`).
- **Palabras del efecto de tipeo**: array `words` en el `<script>` al final.
- **Proyectos**: duplica un bloque `<article class="card">` en la sección `#projects`.
- **Activar un proyecto "IN PROGRESS"**: cuando subas el repo, en su tarjeta
  reemplaza `<span class="repo-link soon">Repo Coming Soon</span>` por
  `<a class="repo-link" href="URL_DEL_REPO" target="_blank" rel="noopener">View Repo →</a>`
  y borra el `<span class="wip">● IN PROGRESS</span>` (hay un comentario en el HTML como recordatorio).
- **Stats**: cambia `data-target` en los contadores de la sección `#stats`.
- **LinkedIn**: añade tu URL en los botones de contacto si quieres incluirlo.
