# MOON64 Residencial · visor tipo libro

Visor estático (HTML + JavaScript) con pase de páginas: portada y contraportada rígidas y dobles páginas (2-3, 4-5 … 46-47) que se ven abiertas como en el libro impreso. En un móvil en vertical se muestra de página en página; en horizontal se ve el libro abierto.

## Publicación

GitHub Pages: **Settings → Pages → Deploy from a branch → `main` / `(root)`**.

## Estructura

- `index.html`: el visor. Al principio del `<script>` está el bloque `CONFIGURACIÓN` (título de la pestaña, número de páginas, carpeta y extensión).
- `paginas/001.webp … 048.webp`: las 48 páginas, renderizadas desde el PDF a 3000 px de ancho.
- `libs/page-flip.browser.js`: librería de efecto libro ([StPageFlip](https://github.com/Nodlik/StPageFlip), MIT).

## Controles

Clic o arrastre en una página o esquina, deslizar en móvil, flechas ← →, `Inicio` / `Fin` y `F` para pantalla completa.

## Cambiar páginas

Sustituye los archivos de `paginas/` conservando los nombres (`001.webp`…). Si cambia el número de páginas, actualiza `total` en `index.html` (ahora 48). La portada (001) y la contraportada (la última) son las páginas rígidas. Para que las dobles páginas sigan emparejadas, mantén un número par de páginas.

## Nota

El repositorio es público, así que las imágenes de las páginas también lo son.
