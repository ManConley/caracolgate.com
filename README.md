# Cara Colgate, LICSW — Astro Site

## Project Structure

```
src/
  layouts/
    Base.astro          ← shared header, nav, footer (edit nav/footer here)
  pages/
    index.astro         ← Home
    about.astro         ← About Me
    children-teens.astro ← Children & Teens
    adults.astro        ← Adults
    more-info.astro     ← More Info
    connect.astro       ← Connect (contact form)
  styles/
    global.css          ← CSS variables, typography, base styles
public/
  images/               ← Place your image files here (see below)
  favicon.svg
```

## Images Needed

Place these image files in `public/images/`:

| Filename              | Used on         | Description                        |
|-----------------------|-----------------|------------------------------------|
| `hero-path.jpg`       | Home            | Boardwalk through green marshland  |
| `cara-headshot.jpg`   | About Me        | Cara's portrait photo              |
| `children-hands.jpg`  | Children & Teens | Adult + child hands (B&W)         |
| `adults-stones.jpg`   | Adults          | Stacked stones by the ocean        |
| `office.jpg`          | More Info       | Therapy office interior            |
| `connect-fern.jpg`    | Connect         | Unfurling fern frond               |

## Getting Started

```bash
npm install
npm run dev       # starts dev server at http://localhost:4321
npm run build     # builds to ./dist/
npm run preview   # preview the production build
```

## Deploying to Netlify (recommended — free)

1. Push this folder to a GitHub repository
2. Go to [netlify.com](https://netlify.com) → "Add new site" → "Import from Git"
3. Set build command: `npm run build`
4. Set publish directory: `dist`
5. Click Deploy — Netlify will give you a URL and you can point your domain to it

The contact form uses Netlify Forms (the `data-netlify="true"` attribute on the form).
It works automatically once deployed to Netlify — no backend needed.

## Deploying to GitHub Pages (also free)

Install the Astro GitHub Pages adapter:
```bash
npm install @astrojs/github-pages
```
Then follow: https://docs.astro.build/en/guides/deploy/github/

## Customizing

- **Nav links / site name**: edit `src/layouts/Base.astro`
- **Colors / fonts**: edit `src/styles/global.css` CSS variables at the top
- **Footer text**: edit the `<footer>` in `src/layouts/Base.astro`
- **Page content**: edit the corresponding `.astro` file in `src/pages/`
