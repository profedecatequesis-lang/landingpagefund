# Fundación Freinet — Sitio institucional

Sitio estático construido con [Astro](https://astro.build). Publicado automáticamente con **GitHub Pages** en:

👉 https://profedecatequesis-lang.github.io/landingpagefund/

## Desarrollo

```sh
npm install
npm run dev      # servidor local en http://localhost:4321
npm run build    # genera ./dist
npm run preview  # vista previa del build
```

## Publicación

Cada push a `main` ejecuta el workflow `.github/workflows/deploy.yml`, que compila el sitio y lo despliega en GitHub Pages (origen: GitHub Actions).

> Nota: los enlaces internos usan `import.meta.env.BASE_URL` (ver `astro.config.mjs` → `base: '/landingpagefund/'`) para que funcionen tanto en local como en Pages.
