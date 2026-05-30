# lidiaymanolo.com

Invitación de boda · 6 de diciembre de 2026 · Málaga.

Estática, una sola página, desplegada en GitHub Pages con dominio propio.

## Estructura

- `index.html` — toda la página (HTML, CSS y SVG inline).
- `og-preview.jpg` — previsualización por defecto (español) para WhatsApp / redes.
- `og-preview-<code>.jpg` — previsualizaciones por idioma (ca, en, nl, ro, ru, ar).
- `lang/<code>/index.html` — páginas estáticas con OG por idioma que redirigen al idioma elegido.
- `CNAME` — dominio personalizado para GitHub Pages.

## Idiomas y enlaces compartibles

Para que WhatsApp muestre la previsualización en el idioma adecuado, compártase la URL del idioma:

| Idioma  | URL                                  |
| ------- | ------------------------------------ |
| Español | `https://lidiaymanolo.com/`          |
| Català  | `https://lidiaymanolo.com/lang/ca/`  |
| Deutsch | `https://lidiaymanolo.com/lang/de/`  |
| English | `https://lidiaymanolo.com/lang/en/`  |
| Nederl. | `https://lidiaymanolo.com/lang/nl/`  |
| Română  | `https://lidiaymanolo.com/lang/ro/`  |
| Русский | `https://lidiaymanolo.com/lang/ru/`  |
| العربية  | `https://lidiaymanolo.com/lang/ar/`  |

Al hacer clic, la página redirige al index principal con el idioma cargado. Dentro de la app, el dropdown de idiomas también actualiza la URL al patrón `/lang/<code>/`.

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
