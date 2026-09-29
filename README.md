# TALK YOUR SH*T — Webinar Landing Page

Free live training with Jamie Arrigo. Registration page for the Oct 1, 12 PM ET webinar.

## Project Structure

```
talk-your-shit/
├── index.html          # Landing page (standalone HTML/CSS)
├── assets/             # Image assets (ocean hero, Jamie headshot)
├── package.json         # Minimal — for wrangler/local dev
├── wrangler.jsonc       # Cloudflare Pages config
└── README.md           # This file
```

## Deployment

### Cloudflare Pages

1. `npx wrangler pages deploy . --project-name=talk-your-shit`
2. Or connect this GitHub repo to Cloudflare Pages dashboard for automatic deploys on push.

### Local Preview

```bash
npx wrangler pages dev .
# or just open index.html in a browser
```

## Notes

- **Fonts**: Uses EB Garamond (headline fallback for Advercase), Archivo (body), IBM Plex Mono (labels) via Google Fonts. If Advercase webfont files are supplied, replace the Google Fonts link in `index.html`.
- **Form**: Preview only — not connected to any email provider. Integration details needed.
- **Assets**: Ocean hero image and Jamie's headshot are placeholders. Replace files in `assets/` when supplied.
- **Editorial notes in source copy**: The Andrew Kaufman testimonial contained an embedded editorial note ("we could add how he stopped using social because he thought he was shadow banned to getting 100K new followers and 5k leads per month"). This was not included in the published text — flagged here for Jamie's review.
