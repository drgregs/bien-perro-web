# Bien Perro — Taquería

Static one-page site for Bien Perro, a Mexican taquería in Madrid.

Bilingual (ES/EN) with a client-side language toggle, animated ticker, scroll reveals
and a fully responsive layout. No build step, no dependencies — a single `index.html`
with inline CSS and JS. Fonts load from Google Fonts.

## Local preview

Open `index.html` in a browser, or serve it:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000

## Deploy to Netlify

The site is static, so there is nothing to build:

- **Build command:** _(leave empty)_
- **Publish directory:** `.`

Both are already set in `netlify.toml`. Connect the repo in Netlify
(Add new site → Import an existing project → GitHub) and it deploys on every
push to `main`.

## Editing

Everything lives in `index.html`:

- Colours are CSS custom properties in the `:root` block at the top.
- Bilingual copy uses paired `<span class="es">` / `<span class="en">` elements —
  edit both when changing text.
- The ticker strings are duplicated in the `<script>` block (`es` and `en` arrays).
