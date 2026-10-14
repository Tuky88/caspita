# CÁSPITA.Custom — sitio web

Sitio estático (HTML + CSS + JS, sin build) de **CÁSPITA.Custom**, taller de tenis, chamarras y tote bags pintados a mano en la CDMX.

- Instagram: [@_caspitacustom_mx](https://www.instagram.com/_caspitacustom_mx/)
- Facebook: [caspita25](https://www.facebook.com/caspita25)
- WhatsApp: 55 1534 1803 (`https://wa.me/525515341803`)

## Estructura

```
index.html   página completa (estilos y script incluidos)
img/         fotos en WebP (miniatura `*-t.webp` ~480 px y versión grande ~900 px), logo y favicon
CHANGELOG.md historial de versiones
```

## Ver en local

```bash
python -m http.server 8000
# abrir http://localhost:8000
```

## Publicar

Sube el contenido tal cual a cualquier hosting estático (GitHub Pages, Netlify, Vercel, Cloudflare Pages o cPanel). Solo hacen falta `index.html` y la carpeta `img/`.

Para GitHub Pages: *Settings → Pages → Deploy from a branch → `main` / root*.

## Editar contenido

- **Galería:** cada foto es un `<button class="pieza" data-cat="...">` dentro de `#galeria-grid`. Categorías: `tenis`, `chamarras`, `bolsas`, `arte`. Para agregar una, sube `img/nombre.webp` y `img/nombre-t.webp` y copia uno de los botones.
- **WhatsApp:** busca `525515341803` para cambiar el número; el texto prellenado va en `?text=`.
- **Colores y tipografías:** variables CSS en `:root` al inicio del `<style>`.

Las fotos provienen de las publicaciones de Instagram del negocio (capturadas el 13 oct 2026).
