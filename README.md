# R&T Deposit Solutions – Temporary Splash Page

A single static page shown on rnt.com while the main WordPress site is offline.

## Develop

```sh
npm install
npm run dev      # http://localhost:4321
npm run build    # outputs to dist/
```

## Deploy (Netlify)

Netlify reads `netlify.toml`: it builds with `npm run build` and publishes `dist/`. A catch-all rewrite sends every path to the splash page.

## Editing

- Copy and the contact email: `src/pages/index.astro`
- Colors, fonts, layout: `src/styles/global.css`
- Hero background, lines and photo are copied from the main site's theme (`rnt-theme/template-parts/gradientBackgrounds/` and the home hero slide image).
