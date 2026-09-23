# Kinetic Kevin

Bare-bones booking / showcase site for Kinetic Kevin’s science-themed birthday and event hosting business.

**Live:** https://kinetickevin.com (also https://kinetickevin.pages.dev while DNS propagates)

**Bookings:** [book@kinetickevin.com](mailto:book@kinetickevin.com)

## Stack

- Static HTML + CSS (no framework)
- Hosted on Cloudflare Pages
- Domain + email routing on Cloudflare

## Local preview

Open `index.html` in a browser, or:

```bash
npx wrangler pages dev .
```

## Deploy

```bash
npx wrangler pages deploy . --project-name kinetickevin --branch main
```

Git-connected deploys (once the GitHub repo is linked in Cloudflare Pages) will publish on push to `main`.

## Filling in content

Replace every `[PLACEHOLDER: …]` and `[PHOTO]` in `index.html` with real copy and images. Put images in an `images/` folder and update the gallery / hero markup accordingly.

See **KEVIN-CHECKLIST.md** for the full handoff list.
