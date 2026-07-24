# Lumen Gallery — Assignment 1

A 9-page online art gallery built with **HTML5, CSS3, and Bootstrap 5**. The theme is a midnight museum wall: dark gallery rooms, brass "track-lighting" gold accents, and framed artwork cards labelled like real museum placards.

## Live Structure (9 pages)

| # | Page | File | Description |
|---|------|------|-------------|
| 1 | Login | `index.html` | Split-screen sign-in form with artwork visual panel |
| 2 | Sign Up | `signup.html` | Split-screen registration form with artwork visual panel |
| 3 | Gallery Home | `gallery.html` | Hero section, three "rooms" (categories), featured works, call-to-action |
| 4 | Art Display | `art-display.html` | Full collection grid — image, artist, category filter pills, link to each piece |
| 5 | Aurora Bloom | `art1.html` | Individual art page |
| 6 | Silent Forest | `art2.html` | Individual art page |
| 7 | Portrait in Amber | `art3.html` | Individual art page |
| 8 | River Flow | `art4.html` | Individual art page |
| 9 | Solstice Glow | `art5.html` | Individual art page |

Each individual art page includes the artwork image, artist name, year of creation, a short description, and 2–3 similar pieces from the same category with links back into the collection.

## Artwork Assets

All artwork is original, hand-built SVG illustration (no external/copyrighted images):

- `aurora.svg` — Aurora Bloom
- `forest.svg` — Silent Forest
- `portrait.svg` — Portrait in Amber
- `river.svg` — River Flow
- `solstice.svg` — Solstice Glow

## Shared Files

- `styles.css` — single shared stylesheet: color tokens, typography, navbar, framed-card component, placard labels, auth layout, detail page layout, and animation keyframes.

## Tech Stack

- **HTML5** — semantic markup across all 9 pages
- **CSS3** — custom design system layered on top of Bootstrap (CSS variables, gradients, keyframe animations)
- **Bootstrap 5.3** (via CDN) — grid system, navbar, forms, breadcrumbs, buttons
- **Vanilla JavaScript** — scroll-reveal animations (IntersectionObserver) and client-side category filtering on the Art Display page
- **Google Fonts** — Playfair Display (headings) + Inter (body/UI)

## Bonus Features Implemented

- Scroll-triggered fade/slide-in reveal animations on every page (respects `prefers-reduced-motion`)
- Hover "spotlight" lift effect on artwork cards (lift, glow border, image zoom)
- Live category filter pills on the Art Display page (Luminous Abstract / Quiet Landscape / Portraiture) — no page reload
- Ambient drifting spotlight glow decoration on the gallery hero
- Consistent breadcrumb navigation on every individual art page
- Fully responsive layout down to mobile (Bootstrap grid + custom breakpoints)

## How to Run

No build step required. Just open `index.html` (or any page) directly in a browser, or serve the folder with any static file server:

```bash
npx serve .
# or
python3 -m http.server
```

## Notes

Per assignment instructions, **no form validation** is implemented on the Login or Sign Up pages — forms are visual/UI only at this stage.
