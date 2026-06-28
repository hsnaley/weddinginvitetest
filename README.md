# House of Saima — Wedding Invitation (Lahore)

A bespoke, cinematic digital wedding invitation. Static site (single `index.html`), deployed on Vercel.

## Structure
- `index.html` — the entire invitation (HTML, CSS, JS inline)
- `assets/cine/` — videos (`*_web.mp4`), poster stills (`*_poster.webp`), background images (`*_bg.webp`), and music
- `vercel.json` — long-cache headers for `/assets`

## Editing
All content lives in the `CONFIG` object near the top of `index.html` (couple, dates, events, venues, RSVP number). Change those values to reuse this template for another couple.

## Performance rules (keep these)
- Photos = **WebP**, never PNG.
- Below-the-fold `<img>` get `loading="lazy"`.
- Each scene has a `*_poster.webp` so a still shows instantly; videos preload ~2.5 viewports ahead.

Deploys automatically to Vercel on every push to `main`.
