+++
title = "Getting Started"
date = 2026-03-16T08:00:00+01:00
weight = 10
kicker = "Foundation"
lead = "Start with a handbook structure that stays easy to edit in Markdown and still feels credible when published in public."
description = "How to structure a public Helixiora handbook in Hugo."
+++

## What this handbook should do

The public handbook is not a dumping ground for internal notes. It should explain how Helixiora thinks, what it ships, and how people can work with the company without forcing visitors to decode a private wiki.

Three jobs matter most:

1. Frame the company's point of view.
2. Make delivery and publishing practices legible.
3. Keep the surface area small enough that every page can stay sharp.

## Recommended content tree

The structure below is enough to launch with substance while still staying easy to maintain.

```text
content/
  _index.md
  docs/
    _index.md
    getting-started.md
    platform-overview.md
    editorial-standards.md
    publishing-workflow.md
    design-language.md
```

Keep pages distinct. If a topic can fit into a single public answer, it probably does not need its own section.

## Front matter pattern

Each page in this sample handbook uses a minimal front matter contract:

```toml
+++
title = "Page title"
date = 2026-03-16T08:00:00+01:00
weight = 10
kicker = "Category"
lead = "One sharp sentence that explains the page."
description = "Metadata for search and social previews."
+++
```

`weight` controls ordering in the handbook list. `lead` gives each page a clean intro without stuffing the main title.

## A good first publishing pass

Write the first public version as if a new client, peer, or future recruit will land on the site with no prior context.

- Prefer direct language over consultant filler.
- Publish principles and working methods before marketing claims.
- Use examples and concrete artifacts whenever possible.
- Link between pages so the handbook reads as a system.

> If a page would confuse an intelligent outsider, it is not ready for public publication yet.

## What to do next

After the structure is in place, move to the [platform overview](/docs/platform-overview/) and [editorial standards](/docs/editorial-standards/) pages to make the experience coherent.
