
# Bobo — Create Account (HTML + CSS)

Minimal sign‑up card UI with glassmorphism, dark mode, and responsive grid.

## Structure
```text
bobo-signup/
├─ index.html
└─ style.css
```

## Quick Start
1. Put the HTML into `index.html`, CSS into `style.css`.
2. In `<head>` include:
```html
<meta name="viewport" content="width=device-width, initial-scale=1" />
<link rel="stylesheet" href="style.css" />
```
3. Open `index.html` in a browser.

## Features
- Responsive 2‑column → 1‑column at `960px`.
- System dark mode (`prefers-color-scheme`).
- Reduced‑motion friendly (`prefers-reduced-motion`).
- Native HTML validation (labels, `required`, autocomplete hints).

## Customize quickly
- Radius/shadows: tweak `--radius`, `--shadow-*` in `:root`.
- Brand colors: `--primary`, `--accent`.
- Glass blur: `--glass` (`backdrop-filter`).
- Layout: adjust `.card { grid-template-columns: ... }`.

## Notes
- Fix typos:
```html
<!-- change 'viewoprt' → 'viewport' -->
<meta name="viewport" content="width=device-width, initial-scale=1" />
```
```css
/* add missing dot for the pseudo-element selector */
.card::after { /* ... */ }
```
- `novalidate` disables browser error bubbles; remove it to use native messages.

## Troubleshooting
- No styles? Verify the `<link>` path and MIME served as `text/css`.
- Blurry/glass not showing? Ensure browser supports `backdrop-filter`.
- Focus ring: customize via `--ring` and `.field:focus-within ...`.

