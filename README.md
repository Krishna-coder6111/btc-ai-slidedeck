# btc-ai-slidedeck — Slidev slides for BTC + AI

Quick start

- Install dependencies: `pnpm install`
- Run dev server: `pnpm run dev` (opens the slides, default port shown in terminal)
- Build static site: `pnpm run build`
- Export PDF/HTML: `pnpm run export`

Notes

- Slide source: [slides.md](slides.md)
- Public assets: put images and static files in the `public/` folder and reference them as `/filename` (served at the site root).
- Theme: uses `@slidev/theme-bricks` and UnoCSS via Slidev.

Deploy

- GitHub Pages: push to the `main` branch and the included workflow will build the slides and publish them automatically.
- Netlify / Vercel: connect the repo and set the build command to `pnpm run build` and publish directory to `dist/`.

More

- Edit the slides in [slides.md](slides.md). See Slidev docs: https://sli.dev/

