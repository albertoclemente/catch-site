# Catch — beta landing page

One page, no build step, no dependencies. Open `index.html` and it works.

- Six languages (EN/IT/JA/ZH/KO/AR): every translatable node carries one `data-<lang>` attribute
  per language, and the toggle swaps them. Arabic sets `dir="rtl"` on `<html>`, so the whole page
  mirrors rather than just the text. The choice is remembered in `localStorage`; a first visit
  walks `navigator.languages` and takes the first supported base tag — `zh-Hant` and `zh-Hans`
  both land on the one Chinese, as they do in the app — and falls back to English.
- The shelf demo is the point of the page. Five foods fade at different rates as the slider
  advances — greens first, oil last — which is the app's own per-food-group freshness model,
  compressed from weeks into a drag. It exists because the fade cannot be filmed.
- Colours and type come from the "Organic" design system on Claude Design, with one deliberate
  departure: the primary button keeps the app's own coral so the button on the page is the
  button in the app.
- The contact form builds a `mailto:` and stores nothing. The page has no backend and sets no
  cookies, which is why it needs no consent banner.

Deployed from `main` via GitHub Pages.
