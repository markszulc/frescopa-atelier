# Fréscopa — The Atelier

Standalone project for the **Atelier** homepage direction: a warm, editorial
flagship for Fréscopa (a fictional premium coffee/tea brand created for demo
purposes). This repo was split out from the multi-direction concept picker
`frescopa-homepage-concepts` on 2026-07-13 so it can be iterated on independently.

## Design identity

- **Direction:** warm editorial flagship — considered, not tech-y.
- **Type:** Schibsted Grotesk (headlines) + Hanken Grotesk (body & labels).
- Sibling project: **Craft & Current** (bold, drenched colour) lives in its own
  separate repo — this project shares no files with it.

## Structure

Everything this project needs lives inside this folder — no dependency on any
sibling `shared/` or `assets/` folder elsewhere.

```
.
├── index.html          # the Atelier homepage
├── atelier.css
├── server.mjs          # zero-dependency static server (serves this folder)
├── shared/             # design system: tokens, reveal/header/nav/calendar JS,
│                       #   Flavour DNA, art-directed hero — a LOCAL copy
├── assets/             # only the images + logo variants this direction uses
└── atelier-pdp/        # the Atelier product detail page (served at /atelier-pdp/)
```

## Running it

```bash
node server.mjs          # serves this folder at http://localhost:4173
```

Any static server works; `server.mjs` is a zero-dependency helper that serves
whatever folder it lives in. The homepage is at `/`, the PDP at `/atelier-pdp/`.

## Conventions

- Plain HTML, CSS, and vanilla JS — **no build step**. Markup is block-shaped
  for a mechanical lift into Adobe Edge Delivery Services (EDS).
- The `shared/` folder is a **local, independent copy**. Edit freely; it is not
  linked to the Craft & Current project or the original concept picker.
- **Imagery:** generate with Adobe Firefly — do not use stock or placeholder
  images.
- Keep the tone warm and human, not tech-forward.

---

*Fréscopa is a fictional brand created for demonstration purposes only.*
