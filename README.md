# Helixiora Handbook

A public-facing Hugo handbook with Helixiora-inspired branding, sample documentation pages, and a GitHub Pages deployment workflow.

## Run locally

```bash
hugo server
```

The local site will be available at `http://localhost:1313/`.

## Build for production

```bash
hugo --gc --minify
```

## Publish on GitHub Pages

This repository includes `.github/workflows/hugo.yml`, which builds the site and deploys it to GitHub Pages.

To publish:

1. Push this repository to GitHub.
2. In the repository settings, enable GitHub Pages and select **GitHub Actions** as the source.
3. The workflow will build the site with the correct Pages base URL automatically.

## Content structure

- `/content/_index.md` powers the landing page.
- `/content/docs/` contains the public handbook pages.
- `/assets/css/main.css` controls the custom visual system.
- `/layouts/` contains the Hugo templates and reusable partials.
