+++
title = "Publishing Workflow"
date = 2026-03-15T08:15:00+01:00
weight = 40
kicker = "Delivery"
lead = "Publishing should be operationally lightweight: edit Markdown, review the diff, merge to main, and let GitHub Pages deploy the static site."
description = "How the Helixiora handbook should be published with Hugo and GitHub Pages."
+++

## Workflow summary

This repository already includes a GitHub Pages workflow, so the publishing path can stay simple:

1. Edit or add content in `content/docs/`.
2. Run `hugo server` locally and review the rendered page.
3. Open a pull request with the content and design changes.
4. Merge to `main`.
5. Let GitHub Actions build and publish the site.

## What the workflow deploys

The included workflow builds the static site with a Pages-specific base URL:

```yaml
- name: Build
  run: hugo --gc --minify --baseURL "${{ steps.pages.outputs.base_url }}/"
```

That keeps the site portable across user pages, project pages, and custom domains.

## Recommended operating rhythm

Treat handbook publishing like software delivery:

- Batch related changes into coherent pull requests.
- Review wording and layout together.
- Keep page titles stable so links do not churn unnecessarily.
- Publish small updates often instead of redesigning everything in one pass.

## Release checklist

Before merging, check the following:

- The page title is clear in navigation cards and browser tabs.
- Tables, code blocks, and links render cleanly on mobile.
- The lead paragraph explains the page in one sentence.
- New pages have a `weight` so the handbook ordering stays intentional.

## Future extension

Once the site is live, it can grow into release notes, essays, capability pages, or public methods docs without changing the base layout.
