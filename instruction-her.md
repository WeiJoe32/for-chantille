# instruction-her

> ⚠️ This repo is public (GitHub Pages). Nothing in this file that isn't already visible on the live site.

## What it is
A one-page "will you be my girlfriend?" site. Scanned from an NFC tag → opens on her phone.

**Flow:** question → No leads through escalating "are you sure?" screens (No shrinks, Yes grows) → final screen only offers Yes → confetti congrats screen with a line-art couple badge, a message, and a photo spot.

## Files
| File | Purpose |
|------|---------|
| `index.html` | The whole site — inline CSS + JS, no build step, no dependencies (Google Fonts only) |
| `photo.jpg` | Optional — drop a square-ish photo with this exact name and it auto-replaces the "photo coming soon" circle |
| `instruction-her.md` | This file |

## Run locally
Open `index.html` in any browser. Test at mobile size (Chrome DevTools → device mode, 390×844).

## Deploy
- Repo: `WeiJoe32/for-chantille` → GitHub Pages from `master`, root
- Live: https://weijoe32.github.io/for-chantille/
- Update = commit + push; Pages redeploys in ~1 min.

## How to edit before the day
1. **Photo:** put `photo.jpg` in this folder → commit + push. No code change needed.
2. **Message:** in `index.html`, find `id="love-msg"` and edit the text between the tags.
3. **Question texts:** in `index.html`, find `const steps` — each line is one screen.

## NFC (manual step)
Write `https://weijoe32.github.io/for-chantille/` to the tag with the usual NFC writer app on the phone. Test-scan before giving it to her.
