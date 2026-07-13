# Fréscopa — The Atelier

Standalone homepage for the **Atelier** direction (warm editorial flagship).
Split out into its own repo from the multi-direction concept picker
[`frescopa-homepage-concepts`](https://github.com/markszulc/frescopa-homepage-concepts)
on 2026-07-13 so it can be iterated on independently.

Type: **Schibsted Grotesk** (headlines) + **Hanken Grotesk** (body & labels).

## View it

```bash
node server.mjs          # serves this folder at http://localhost:4173
```

Any static server works; `server.mjs` is a zero-dependency helper that serves
whatever folder it lives in. Homepage at `/`, product page at `/atelier-pdp/`.

## Structure

Everything this direction needs lives inside this folder — no dependency on
a sibling `shared/` or `assets/` folder elsewhere.

```
.
├── index.html          # the Atelier homepage
├── atelier.css
├── server.mjs
├── shared/             # design system (tokens, reveal/header/nav/calendar JS, Flavour DNA, art-directed hero)
├── assets/             # only the images + logo variants this direction actually uses
└── atelier-pdp/        # the Atelier product detail page
```

## Notes

- Plain HTML, CSS, and vanilla JS — no build step, block-shaped markup for a
  mechanical lift into Adobe Edge Delivery Services.
- `shared/` here is a **local, independent copy** — not linked to the
  Craft & Current project or the original concept picker.

---

*Fréscopa is a fictional brand created for demonstration purposes only.*
