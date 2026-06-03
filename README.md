# Seitenwerk.de — kuechenstudio Landing Page

Seitenwerk.de — Websites für Küchenstudios mit Anspruch

> Generated from a Claude Design handoff and implemented with Claude Code. Design from Claude Design; content from the handoff HTML.

A single, self-contained static landing page — light theme, German copy, no build step.

## Tech stack

- Plain HTML + CSS (`seitenwerk-kitchen.css`) — design tokens via CSS custom properties
- Vanilla JS (inline): scroll-progress bar, IntersectionObserver scroll-reveals, single-open FAQ accordion, 3D hero-mockup tilt + floating-chip parallax
- Typography: Inter Tight (Google Fonts)
- Respects `prefers-reduced-motion`; reveals are print/no-JS safe

## Project structure

```
index.html          # the page
seitenwerk-kitchen.css
favicon.svg
404.html            # on-brand fallback
assets/og.png       # social preview
```

## Local development

```bash
npx serve .          # or: python3 -m http.server 8000
```

Then open http://localhost:3000 (or :8000).

## Deployment

- **GitHub Pages** — served from `main` branch root → https://aiaccountsc.github.io/seitenwerk-kuechenstudio/
- **Netlify** — zero-config via `netlify.toml` (publish = ".")
- Any static host works (no build).

## License & usage

Brand name, copy and visual identity © Seitenwerk.de. The underlying template/code is free to reuse.
