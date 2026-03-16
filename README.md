# Helixiora Employee Handbook

A Hugo employee handbook with Helixiora-inspired styling, sample HR and operations pages, and a GitHub Pages deployment workflow.

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
3. Point the DNS for `handbook.helixiora.com` at GitHub Pages.
4. The workflow publishes with the custom domain `https://handbook.helixiora.com/`.

## Content structure

- `/content/_index.md` powers the landing page.
- `/content/docs/` contains the employee handbook pages.
- `/assets/css/main.css` controls the custom visual system.
- `/layouts/` contains the Hugo templates and reusable partials.

## License

The Helixiora Employee Handbook content in this repository is licensed under the
[Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)
license. You are free to share and adapt the material, provided you give appropriate
credit and indicate if changes were made.

## Contributing

Contributions and improvements are welcome.

- **Propose changes**: Open a pull request with clear, concise commits and a short
  description of what you are changing and why.
- **Report issues**: If you spot mistakes, omissions, or unclear guidance, open an
  issue describing the problem and, if possible, suggest how it could be improved.
- **Style and tone**: Keep additions practical, employee-focused, and easy to scan.
