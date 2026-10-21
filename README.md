# Daily Budget

A small offline app for recording what I spend each day against a daily budget. Built for iPhone as a home-screen web app — no account, no internet needed, data stays on the phone.

## Features

- Set a daily budget and currency symbol
- Add expenses with a category and optional note; tap an entry to edit or delete it (with undo)
- See what's left today, with a ring that turns orange near the limit and red when over
- Go back to earlier days to record or review them
- Monthly history: total spent, budget, saved/overspent, daily average, days within budget, spending by category
- Export a CSV spreadsheet, save a JSON backup, restore from a backup

## Install on iPhone

1. Open **https://fmsami.github.io/daily-budget/** in **Safari** (must be Safari).
2. Tap **Share** → **Add to Home Screen** → **Add**.
3. Open it once from the home screen while online. After that it works fully offline.

## Files

- `index.html` — the whole app (HTML, CSS, JS)
- `sw.js` — service worker that caches the app for offline use
- `manifest.webmanifest`, `icons/` — home-screen name and icons

When changing the app, bump `CACHE` in `sw.js` so phones pick up the new version.
