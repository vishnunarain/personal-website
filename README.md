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

## Editorial design

The front page leads with the newest published featured field note, with the newest note as fallback. Set `featured: true` to promote a story. Optional `cover` and `coverAlt` fields supply its illustration. Existing `/imho` and `/tep` routes remain available as Marginalia and The work.

The Imhotep character is a fictional stick-figure polymath. The inaugural dispatch is an invented fable, not a historical account. The cover is a static illustration in the style of a colourful history animation, with restrained hover motion and reduced-motion support.

Artwork: generated using the built-in image generator. Brief: colourful hand-drawn editorial cartoon of stick-figure Imhotep holding a long blueprint in a dry Nile riverbed, a step pyramid under construction, stranded boat and waiting builders; turquoise, ochre, coral and cream; no text. Optimized asset: `public/images/imhotep-nile.webp`.
