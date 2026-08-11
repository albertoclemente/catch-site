# Catch — beta landing page

One page, no build step, no dependencies. Open `index.html` and it works.

- Bilingual EN/IT: every translatable node carries `data-en` / `data-it`, and the toggle swaps
  them. The choice is remembered in `localStorage`; first visit follows the browser language.
- The shelf demo is the point of the page. Five foods fade at different rates as the slider
  advances — greens first, oil last — which is the app's own per-food-group freshness model,
  compressed from weeks into a drag. It exists because the fade cannot be filmed.
- Colours and type come from the "Organic" design system on Claude Design, with one deliberate
  departure: the primary button keeps the app's own coral so the button on the page is the
  button in the app.
- The contact form builds a `mailto:` and stores nothing. The page has no backend and sets no
  cookies, which is why it needs no consent banner.

Deployed from `main` via GitHub Pages.
