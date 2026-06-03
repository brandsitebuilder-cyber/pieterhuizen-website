# Pieterhuizen Planning Website — Rebuild Notes

**Date:** May 17–18, 2026  
**Client:** Pieterhuizen Planning (PTY) Ltd — Town Planning Consultants, Western Cape

## Links

| Resource | URL |
|---|---|
| **Live site (new)** | https://pieterhuizen-website.vercel.app |
| **Original site** | https://pieterhuizen.co.za (WordPress — still live) |
| **GitHub repo** | https://github.com/brandsitebuilder-cyber/pieterhuizen-website |
| **Vercel project** | `brandsitebuilder-9030s-projects/pieterhuizen-website` |
| **Local path** | `/home/marcus/projects/pieterhuizen-website` |

## Tech Stack

- **Framework:** Astro (static site)
- **Styling:** Tailwind CSS v4 (`@import "tailwindcss"` with `@theme`)
- **Font:** Inter (Google Fonts)
- **Deploy:** Vercel, auto-deploy on push to `main`

## Design System (v2 — matched to original site)

| Token | Value | Usage |
|---|---|---|
| `--color-bg` | `#FFFFFF` | Page background |
| `--color-surface` | `#F5F7FA` | Section backgrounds, cards |
| `--color-elevated` | `#EBF0F5` | Elevated surfaces |
| `--color-text` | `#32373C` | Body text |
| `--color-text-secondary` | `#534A45` | Secondary text |
| `--color-text-muted` | `#605F5F` | Muted/helper text |
| `--color-accent` | `#005EB8` | Primary blue (buttons, links, highlights) |
| `--color-accent-hover` | `#004A93` | Button hover |
| `--color-accent-light` | `#8AC4F9` | Light blue accents |
| `--color-accent-gold` | `#F3D97A` | Stars, gold highlights |
| `--color-border` | `rgba(0,0,0,0.08)` | Borders |
| `--color-border-subtle` | `rgba(0,0,0,0.05)` | Subtle borders |

## Logo

- Downloaded from original site: `wp-content/uploads/2021/07/cropped-base_logo_transparent_background-e1625490211962.png`
- Saved to: `public/logo.png` (3125×772px, transparent PNG)
- Shown in nav at `h-9 w-auto`

## Pages (20 total)

- **Home** — hero with gradient bg, stats band, services grid, locations, testimonials, CTA
- **About** — company info
- **Services** (11): rezoning, subdivisions, departures, title deed restrictions, development reports, consolidation, consent use, removal of conditions, zoning compliance, property development, property ownership
- **Service index** — all 11 services in a grid
- **Areas** (4): Cape Town, Somerset West, Stellenbosch, Helderberg
- **Portfolio** — project gallery
- **Contact** — form + details

## Image Situation

- **Original site is image-poor** — only logo + 5 tiny Elementor numbered icons + 3 locality maps
- **No property/project photos exist on original site**
- **Google Drive link shared by Marcus** (logo?) — NOT accessible (needs "Anyone with link" permission): `https://drive.google.com/file/d/161-NnZ0pgtloDUGr-6s8gGFRNBJLdGIP/view`

## History

1. **v1 (May 17):** Dark theme rebuild (~#08090A bg, gold #C8963E accent, Playfair + Inter). Deployed to Vercel.
2. **v2 (May 18):** Color overhaul — matched original WordPress site's blue (#005EB8) + white scheme. Logo added to nav. Pushed and deployed.

## To Do / Notes

- [ ] Marcus to check Google Drive sharing permissions for additional assets
- [ ] May need stock photos (Unsplash/Pexels) for visual appeal — original site has none
- [ ] Domain `pieterhuizen.co.za` still points to old WordPress site; may want to point to Vercel eventually
- [ ] CSS `@import` ordering warning (fonts after Tailwind) — cosmetic, no functional impact
