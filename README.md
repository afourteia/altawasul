# شركة التواصل الحديث لإستيراد الكتب والقرطاسيات

One-page Arabic (RTL) site built with [Astro](https://astro.build).

Live: https://fourteia.com/altawasul/

## Develop

```sh
npm install
npm run dev      # http://localhost:4321/altawasul/
npm run build    # outputs to dist/
```

## Deploy

Every push to `main` builds and publishes the site to GitHub Pages through
`.github/workflows/deploy.yml`. The site is a project page under the
`afourteia.github.io` custom domain, so `astro.config.mjs` sets
`site: 'https://fourteia.com'` and `base: '/altawasul'`.

## Editing content

- Text, products, and contact details live at the top of `src/pages/index.astro`.
- Product pictures are placeholders (`src/components/Placeholder.astro`). To use a
  real photo, add it to `src/assets/` and swap the placeholder for
  `<Image src={photo} alt="..." />` from `astro:assets`.
- Logos in `src/assets/` were cut out of the supplied PDF artwork.
