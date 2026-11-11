# Publicar la landing en GitHub Pages

Esta carpeta contiene todo lo necesario para publicar la landing del **Seminario de Tendencias Deportivas (Martha Toro, Árbitro)** en GitHub Pages:

- `index.html` — landing principal (con logo Uparsistem y simulación integrada)
- `logo-uparsistem.webp` — logo
- `vr-lab/` — laboratorio 3D interactivo (`index.html` embebido en la landing)

> **Nota:** la simulación carga librerías 3D/HDRI desde CDN, por lo que requiere conexión a internet para funcionar correctamente.

## Opción A: Subir desde esta carpeta (recomendada)

1. Crea un repositorio en GitHub (p. ej. `seminario-tendencias-deportivas`). Puede ser público.
2. Abre una terminal **dentro de esta carpeta** (`github-pages`) y ejecuta:

```bash
git init
git add .
git commit -m "Publicar landing seminario tendencias deportivas"
git branch -M main
git remote add origin https://github.com/<TU_USUARIO>/<TU_REPOSITORIO>.git
git push -u origin main
```

3. En GitHub, ve a **Settings → Pages**.
4. En **Build and deployment → Source**, selecciona **Deploy from a branch**.
5. En **Branch**, elige `main` y carpeta **/ (root)**, luego guarda.
6. Espera 1–2 minutos. Tu sitio quedará disponible en:
   - `https://<TU_USUARIO>.github.io/<TU_REPOSITORIO>/`

## Opción B: Usar la carpeta `docs/` en un repositorio existente

1. Copia el contenido de esta carpeta (`index.html`, `logo-uparsistem.webp`, `vr-lab/`) dentro de una carpeta llamada `docs/` en tu repositorio.
2. Sube los cambios (`git add`, `commit`, `push`).
3. En **Settings → Pages**, selecciona rama `main` y carpeta **/docs**.
4. El enlace será: `https://<TU_USUARIO>.github.io/<TU_REPOSITORIO>/`

## Verificación

- Abre el enlace generado y comprueba que se vea el logo, la landing y que el bloque de **Simulación 3D integrada** cargue el laboratorio (`vr-lab/index.html`).
- Si usas un proyecto (no `usuario.github.io`), las rutas relativas incluidas (`logo-uparsistem.webp`, `vr-lab/index.html`) funcionan correctamente en GitHub Pages.
