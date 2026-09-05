# Ronnie’s personal website

An Astro starter for Ronnie’s writing, art, ideas, and projects.

- Website: https://ronnie04nyc.github.io/
- Repository: https://github.com/Ronnie04NYC/Ronnie04NYC.github.io
- Hosting: GitHub Pages, published by GitHub Actions.

## Work locally

Use Node.js 22.12 or newer (Node 22 is recorded in `.nvmrc`).

```sh
npm ci
npm run dev
```

Before publishing, run `npm run check` and `npm run build`.
Use `npm run preview` to view the production build locally.
In a restricted environment, prefix commands with `ASTRO_TELEMETRY_DISABLED=1`.

## Where to edit

- `src/pages/index.astro`: homepage and introductory copy.
- `src/data/site.ts`: name, description, and interests.
- `src/layouts/Base.astro`: shared HTML, metadata, header, and footer.
- `src/styles/global.css`: colors, typography, and responsive layout.
- `public/`: public images and downloadable assets.
- `src/pages/`: add Astro or Markdown files for new pages.

The homepage is intentionally a small starting point. The first design/content
iteration can add verified project links, essays, artwork, and an approved bio.
No Linktree URL, contact address, project destinations, or unpublished essays
have been invented or imported.

## Publishing

GitHub Settings → Pages → Source must be **GitHub Actions**.
Pushes to `main` run checks, build the static site, and deploy `dist/`.
Pull requests run the same checks and build without deploying.
Use a `codex/` branch and a pull request for subsequent design changes.
The Actions tab shows publishing progress and errors.

No hosting secrets, paid services, database, or custom domain are required.
The repository and published site are public: commit only material intended for publication.

The root URL is configured for the special `Ronnie04NYC.github.io` repository.
If moving to another repository, update Astro’s `base` and internal links.
See https://docs.astro.build/en/guides/deploy/github/ for deployment details.
