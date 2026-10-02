# imhotep

Personal website for Vishnu Unnikrishnan, built with Astro.

## Local development

```bash
npm install
npm run dev
```

## Content model

Field notes live in `src/content/field-notes`.

The visible chronology is controlled by frontmatter, not Git history:

```yaml
publishedAt: 2021-06-18
originallyWrittenAt: 2021-06-18
updatedAt: 2026-10-03
draft: false
```

That allows old writing to be added retroactively while preserving the intended date.

## Deployment

The repository is Netlify-ready:

- build command: `npm run build`
- publish directory: `dist`

Before production launch, replace `https://example.com` in `astro.config.mjs` with the final domain.
