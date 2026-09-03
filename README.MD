# tianjiao11.github.io — redesign

A clean, minimal-academic single-page site: `index.html`, with sections for
Home, Research, CV, and Contact. The nav bar links jump to each
section on the same page (smooth-scrolling), rather than loading separate
pages. Shares `css/style.css` and `js/nav.js` (mobile menu toggle, which
also closes itself after you tap a link).

## Deploy

1. Open your `tianjiao11.github.io` repo.
2. Delete `research.html`, `cv.html`, and `contact.html` if they're still
   there from an earlier version — everything now lives in `index.html`.
3. Copy everything in this folder into the repo root, overwriting the old
   `index.html`, `css/`, `js/`, and `images/`.
4. Commit and push to the `master`/`main`/`new` branch (whichever your
   GitHub Pages source is set to). GitHub Pages will publish automatically —
   usually within a minute or two.

No build step, no dependencies — it's plain HTML/CSS/JS, so this works with
GitHub Pages out of the box.

## Status

All sections are filled in — no placeholders left in `index.html`. The
profile photo was intentionally removed (no placeholder image or photo on
the site) — a deliberate choice, not something left unfinished.

## Content carried over from the old site

Everything else (bio, supervisors, department, the published paper, the
working paper, office, and email) was taken directly from the original live
site, so nothing there should need changing.

## Customizing the look

- Colors and fonts are CSS variables at the top of `css/style.css`
  (`--accent` is the oxblood color used for links/tags — change it there to
  re-theme the whole site).
- Dark mode follows the visitor's OS setting automatically (see the
  `prefers-color-scheme: dark` block in the CSS).
- Each section is a `<section id="..." class="container">` block in
  `index.html` — the nav links point at those ids (e.g. `#research`). Adding
  a new section means adding both the `<section>` and a matching `<li><a
  href="#your-id">...</a></li>` in the nav.
