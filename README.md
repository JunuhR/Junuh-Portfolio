# Junuh Ridenour — Web Stack

Two separate sites:

- **`junuh-portfolio/`** — Personal portfolio (dark-mode-first, Apple-style minimal)
- **`ridenour-media-firm/`** — RMF business site rebuild (bold cinematic)

Each folder has its own `index.html` and `README.md` with setup instructions.

## Recommended stack

| Piece | Service | Cost |
|---|---|---|
| Domain registration | Cloudflare Registrar | ~$10/yr for `.com` (at-cost, no markup) |
| Hosting | Cloudflare Pages | Free |
| Contact form | Formspree free tier | Free (50 submissions/mo) |
| Code repo | GitHub | Free |

**Total annual cost: ~$10–25/year** (depending on TLDs chosen)

This beats Carrd Pro ($19/yr) and gives you full code control.

## Domain ideas for personal site

Since RMF already owns `ridenourmediafirm.com`, the personal site needs something separate:

- `junuhridenour.com` — cleanest professional option
- `junuh.dev` — lean into engineering/developer identity
- `junuh.design` — creative/design angle
- `junuh.studio` — creative practice framing
- `builtbyjunuh.com` — maker energy

Check availability at https://domains.cloudflare.com before committing.

## Recommended launch order

1. **Register domain** at Cloudflare Registrar
2. **Create two GitHub repos:** `junuh-portfolio` and `ridenour-media-firm`
3. **Push code** to each
4. **Deploy personal portfolio first** — lower stakes, lets you learn the workflow
5. **Set up Formspree** for RMF (follow `ridenour-media-firm/README.md`)
6. **Deploy RMF to Cloudflare Pages**, test at the `*.pages.dev` URL
7. **Cut DNS over:** point `ridenourmediafirm.com` at the new Cloudflare Pages deployment
8. **Cancel Carrd Pro** after confirming everything works

## Why two repos instead of one

Separate repos mean:
- Each site can be deployed independently (push to personal, RMF doesn't redeploy)
- Future flexibility: if you ever want to hand off RMF dev work, the repo is scoped
- Cleaner commit history per site

## Two distinct aesthetics, on purpose

The sites are intentionally different:

- **Personal portfolio** — refined, typographic, dark default with light toggle. Fraunces serif + mono for engineer identity. Audience: colleges, collaborators, anyone evaluating *you*.
- **RMF** — bold, cinematic, commercial. Bebas Neue display + high-contrast accent. Audience: prospective clients who need to see energy and capability immediately.

Keeping them visually distinct signals you understand branding — a portfolio that looks exactly like your business site suggests you don't differentiate between audiences. This setup shows you do.

## Need to iterate?

Both files are plain HTML/CSS/JS. Edit, save, push to GitHub — Cloudflare Pages auto-deploys on every commit. No build step, no frameworks, nothing to learn.
