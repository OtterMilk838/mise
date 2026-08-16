# Mise

A pantry, shopping list, and recipe app that checks what you can cook
against what you actually have at home.

Open it: **https://ottermilk838.github.io/mise**

- **Offline-first.** One self-contained HTML file, no build step, no server,
  no accounts. Everything runs in the browser.
- **Your data stays on your device.** Pantry, list, and recipes live in the
  browser's local storage and are never uploaded anywhere.
- **Add to Home Screen** on iOS for a standalone app and durable storage.

## What it does

- **Pantry** — what's at home, grouped by location or category, with quick
  +/- adjustments and receipt scanning via iOS Scan Text.
- **Shopping list** — grouped by aisle, with a "buy it again" list built from
  what you've bought before. Checking something off offers to move it into
  the pantry.
- **Recipes** — paste one from any site and it pulls out ingredients and
  steps. Each ingredient is checked against your pantry as have / short /
  missing / amount-unverified, converting units per ingredient using density
  and piece-weight tables. One tap sends what's missing to your list, and
  "I made this" takes the ingredients back out.
- **Cook mode** — one step at a time, large type, with timers detected from
  the text.

Source and tests: the app is generated from `web/mise.html` in the
development repo, wrapped for hosting by `web/build-site.mjs`.
