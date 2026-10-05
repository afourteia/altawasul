# شركة التواصل الحديث لإستيراد الكتب والقرطاسيات

One-page Arabic (RTL) site built with [Astro](https://astro.build).

Live: https://tawasul.net.ly/

## Develop

```sh
npm install
npm run dev      # http://localhost:4321/
npm run build    # outputs to dist/
```

## Deploy

Every push to `main` builds and publishes the site to GitHub Pages through
`.github/workflows/deploy.yml`. The custom domain `tawasul.net.ly` is set in the repo's
Pages settings (no CNAME file is needed with Actions deploys). DNS: apex A/AAAA
records point to GitHub Pages, and `www` is a CNAME to `afourteia.github.io`.

## Editing content

- Text, products, and contact details live at the top of `src/pages/index.astro`.
- Product pictures are placeholders (`src/components/Placeholder.astro`). To use a
  real photo, add it to `src/assets/` and swap the placeholder for
  `<Image src={photo} alt="..." />` from `astro:assets`.
- Logos in `src/assets/` were cut out of the supplied PDF artwork.
