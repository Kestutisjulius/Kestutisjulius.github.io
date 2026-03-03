# Kestutis Skrebe Portfolio (Astro)

Asmeninis CV/portfolio puslapis su `Astro`, pritaikytas publikavimui per `GitHub Pages`.

## Funkcionalumas

- Hero sekcija su kontaktais ir pagrindine informacija
- Patirties, irankiu, kalbu ir issilavinimo blokai
- `Open CV (PDF)` mygtukas, kuris atidaro CV modale
- `favicon` su stilizuota `K` raide (`SVG`) + `ICO` fallback

## Naudojamos technologijos

- `Astro`
- `HTML/CSS`
- `GitHub Actions` (`Pages` deploy)

## Paleidimas lokaliai

```bash
npm install
npm run dev
```

Papildomi skriptai:

```bash
npm run build
npm run preview
```

## Projekto struktura

- `src/pages/index.astro` - visas puslapio turinys ir modal logika
- `public/cv.pdf` - tavo CV failas (butina ideti)
- `public/favicon.svg` - pagrindine favicon ikona
- `public/favicon.ico` - favicon fallback
- `.github/workflows/deploy.yml` - automatinis deploy i `GitHub Pages`
- `astro.config.mjs` - svetaine ir `static` build nustatymai


## Konfiguracija

`astro.config.mjs` dabar nustatytas taip:

```js
export default defineConfig({
  site: "https://kestutisjulius.github.io",
  output: "static"
});
```

Jei keiciasi domenas ar repo strategija, atnaujink `site` reiksme.
