# Daily Budget

A small offline app for recording what I spend each day against a daily budget. Built for iPhone as a home-screen web app — no account, no internet needed, data stays on the phone.

## Features

- Set a daily budget and currency symbol
- Add expenses with a category and optional note; tap an entry to edit or delete it (with undo)
- See what's left today, with a ring that turns orange near the limit and red when over
- Go back to earlier days to record or review them
- Monthly history: total spent, budget, saved/overspent, daily average, days within budget, spending by category
- Export a CSV spreadsheet, save a JSON backup, restore from a backup
- **Savings jar:** set a goal; every night the jar fills with whatever wasn't spent that day, with an estimate of when the goal will be reached
- **Rollover mode** (alternative to the jar): unspent money is spread over the rest of the month, so today's "safe to spend" grows when you save and shrinks after overspending
- **Streaks:** days in a row under budget, plus best streak
- **Price in work time:** enter your hourly income and every amount also shows how many hours of work it cost
- **One-tap repeats:** things bought at least twice recently appear as quick-add buttons
- **Calendar:** each day colored by spent nothing / under / close / over
- **Insights:** month-end forecast, small habits projected over a year, biggest expense, the weekday you spend most
- Weekly reminder to save a backup
- **Trips:** one total budget per trip with dates, a per-day allowance for the days left, and its own categories (Stay, Tickets…). Add travel companions to record who paid and who shares each cost; the app works out who owes who with the fewest payments. Trip spending is kept out of the daily budget.
- **Bills:** monthly bills with a due day; reminders on the Today screen 3 days before, one tap to mark paid. Kept out of the daily budget.
- **Lend & borrow:** borrowed money goes into a wallet and comes out when repaid (lending is the reverse); part payments supported
- **Everything stays in sync:** every change redraws every screen, trip pay-backs move real money, removing a wallet moves its balance, and you're warned when a wallet goes below zero
- **Search** across all expenses, trips and bills
- **Your own categories** with any emoji
- **PIN lock:** asks for a 4-digit PIN on open and after 30 seconds away
- **Wallets & income:** Cash, bKash, Bank… with live balances; record money in, move money between wallets, correct a balance
- **Regular money in:** e.g. pocket money every 2 days — added to your wallet automatically on the day it's due, and can set your daily budget (amount ÷ days)
- **Funds:** regular money for one thing only (e.g. refuel money every 10 days → ⛽ Fuel fund); spending in that category comes out of the fund, not the daily budget
- **Monthly category limits** with warnings on the Today screen
- **Charts:** last 30 days (with the budget line) and last 12 months
- **Type to add:** "tea 20" or "uber 250" — the category is guessed from past entries and keywords
- **Mood:** rate each day, and an insight shows whether you spend more on good or bad days
- **Achievements:** 18 badges for streaks, saving, trips, bills and more
- **Wishlist** with a one-week cooling-off period and "days of saving" for each item
- **Hide amounts** privacy mode, **5 neon color themes**, shareable month summary, evening reminder when nothing is logged
- Premium look: dark navy header on a blueprint grid with a white content sheet, italic serif headings, black selected pills, blue buttons, floating white tab bar
- Opening animation (the logo draws itself), intro screen with a collage, and a welcome/setup screen for first-time users
- 5 accent colors (blue, violet, green, orange, pink)

## Install on iPhone

1. Open **https://fmsami.github.io/daily-budget/** in **Safari** (must be Safari).
2. Tap **Share** → **Add to Home Screen** → **Add**.
3. Open it once from the home screen while online. After that it works fully offline.

## Files

- `index.html` — the whole app (HTML, CSS, JS)
- `sw.js` — service worker that caches the app for offline use
- `manifest.webmanifest`, `icons/` — home-screen name and icons

When changing the app, bump `CACHE` in `sw.js` so phones pick up the new version.
