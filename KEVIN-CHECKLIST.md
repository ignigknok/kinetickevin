# Kevin checklist — Kinetic Kevin site

Hand this list to Kevin (or his agent). Items marked **done for you** are already set up; the rest need Kevin’s input or action.

## Already done (by Tim)

- [x] Placeholder site deployed on Cloudflare Pages → https://kinetickevin.pages.dev
- [x] Custom domains `kinetickevin.com` + `www` attached to Pages (DNS records still need to be confirmed in Cloudflare — see Tim note below)
- [x] Email Routing enabled for the zone
- [x] `book@kinetickevin.com` rule created (currently forwards to Tim’s Gmail until Kevin verifies)
- [x] Destination address invited for **kevinslattery90@gmail.com** (needs Kevin to click verify)
- [x] GitHub repo: https://github.com/ignigknok/kinetickevin
- [ ] Collaborator invite (needs Kevin’s GitHub **username** — no account found for kevinslattery90@gmail.com yet)

## Kevin: content (edit the site)

Work in `index.html` (and add files under `images/` as needed). Every `[PLACEHOLDER: …]` is intentional blank copy.

1. [ ] Write the homepage headline and one supporting sentence
2. [ ] Write the About section (who you are, what guests experience)
3. [ ] List real event offerings / packages (names, ages, length, what’s included)
4. [ ] Add real photos (hero + gallery) — no AI art; use your own event photos
5. [ ] Fill booking details: lead time, travel / service area, what to put in an inquiry email
6. [ ] Add city / service area (and optional phone) in the footer
7. [ ] Optional: favicon, social preview image, Google Business / Instagram links

## Kevin: GitHub access

1. [ ] Create a GitHub account (use **kevinslattery90@gmail.com**) and tell Tim your **username**
2. [ ] Accept the collaborator invite Tim sends for https://github.com/ignigknok/kinetickevin
3. [ ] Clone, edit placeholders, push to `main`
4. [ ] Optional: Tim can transfer the repo to Kevin’s account later so he owns it outright

## Kevin: email (`book@kinetickevin.com`)

Cloudflare Email Routing forwards mail; it does not host a mailbox by itself.

1. [ ] Open Gmail for **kevinslattery90@gmail.com** and click Cloudflare’s destination verification link
2. [ ] Ask Tim to switch the `book@` forward from Tim’s inbox → Kevin’s Gmail (or forward to both)
3. [ ] Send a test message to `book@kinetickevin.com` and confirm it arrives
4. [ ] Optional later: set up a real mailbox (Google Workspace / Microsoft 365) if you want to *send as* book@ from that address

## Kevin: domain / business (optional but useful)

1. [ ] Confirm nameservers for `kinetickevin.com` stay on Cloudflare
2. [ ] Decide whether `www.kinetickevin.com` should redirect to the apex (recommended)
3. [ ] Add a simple privacy / cancellation note if you take deposits later
4. [ ] Connect a real booking calendar (Cal.com, Google Calendar appointment slots, etc.) when ready — replace the mailto CTA

## Owner / sibling notes (Tim)

- [ ] In Cloudflare DNS for `kinetickevin.com`, ensure:
  - `CNAME` apex / `www` → `kinetickevin.pages.dev` (proxied) — Pages UI “Custom domains” can add these if OAuth lacks zone:edit
  - Email Routing MX + SPF + DKIM records (Email Routing UI → “Destination addresses” / DNS setup)
- [ ] Re-auth Wrangler with **zone DNS edit** if you want CLI DNS control (`wrangler login`)
- Cloudflare account currently owns the domain + Pages project
- Transfer zone ownership or add Kevin as a Cloudflare account member when he’s ready to self-serve DNS/email
- Link the GitHub repo to the Pages project for push-to-deploy
