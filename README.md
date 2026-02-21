# D2R LAN Party Tracker

A single-page Diablo II: Resurrected run tracker for LAN parties, designed to be displayed on a TV.

## Features

- **Large central timer** — start, stop, and reset the run clock. State survives page refreshes.
- **Milestone lap times** — mark completion of Normal, Nightmare, and Hell. Shows elapsed time and split (delta from previous milestone).
- **Item tracker** — quickly log Unique (orange) and Set (green) items found. Items show the time they were found.
- **Diablo 2 theme** — dark background, gold text, Cinzel Decorative font, glowing timer.
- **Keyboard shortcuts** — `Space` toggles start/stop; in the item field `Enter` adds a Unique item, `Shift+Enter` adds a Set item.
- **Fully client-side** — all state stored in `localStorage`, no server required.

## Local development

```sh
npm start
# opens http://localhost:3000
```

## Deploy to Cloudflare Pages

### Option A — Dashboard (drag-and-drop)

1. Go to [Cloudflare Pages](https://pages.cloudflare.com/) → **Create a project** → **Direct upload**.
2. Upload the repository folder (or just `index.html`).
3. Done — Cloudflare provides a public URL instantly.

### Option B — Connect GitHub repo

1. Push this repo to GitHub.
2. In Cloudflare Pages, choose **Connect to Git** and select the repo.
3. Set **Build output directory** to `/` (root) and leave the build command blank.
4. Deploy.

### Option C — Wrangler CLI

```sh
npm run deploy
```

(Requires a Cloudflare account and `wrangler login` beforehand.)
