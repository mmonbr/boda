# lidiaymanolo.com

Invitación de boda · 6 de diciembre de 2026 · Málaga.

Estática, una sola página, desplegada en GitHub Pages con dominio propio.

## Estructura

- `index.html` — toda la página (HTML, CSS y SVG inline).
- `og-preview.jpg` — imagen para previsualización en WhatsApp / redes (1200×630).
- `CNAME` — dominio personalizado para GitHub Pages.

## Despliegue

1. En **Settings → Pages** del repo: elegir `main` como branch y `/ (root)` como carpeta.
2. **Custom domain**: `lidiaymanolo.com`. Activar **Enforce HTTPS**.
3. DNS del dominio:
   - `A` `@` → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `CNAME` `www` → `mmonbr.github.io`

## Local

Abre `index.html` directamente o sirve la carpeta con cualquier servidor:

```bash
python3 -m http.server 8000
```
