# tianjiao11.github.io — redesign

A clean, minimal-academic 4-page rebuild of the site: `index.html` (Home),
`research.html`, `cv.html`, `contact.html`, sharing `css/style.css` and
`js/nav.js` (mobile menu toggle).

## Deploy

1. Open your `tianjiao11.github.io` repo.
2. Delete the old `index.html`, `css/`, `js/`, and `images/` (or just replace
   them — the new files use the same names).
3. Copy everything in this folder into the repo root.
4. Commit and push to the `master`/`main` branch. GitHub Pages will publish
   the new site automatically — usually within a minute or two.

No build step, no dependencies — it's plain HTML/CSS/JS, so this works with
GitHub Pages out of the box.

## Things to fill in

A few spots are intentionally left as placeholders rather than guessed, so
you don't end up with invented dates or degrees. Search each file for
`class="placeholder"` or `[start year]`:

- **`index.html`** — swap `images/profile-placeholder.svg` for an actual
  photo (drop a `profile.jpg` into `images/` and update the `src`).
- **`cv.html`** — PhD start year, earlier degrees, positions/experience,
  awards, and skills.
- **`research.html`** — talks, seminars, or other work you want listed.
- **`contact.html`** — Google Scholar, ORCID, LinkedIn, or a CV PDF link.

## Content carried over from the old site

Everything else (bio, supervisors, department, the published paper, the
working paper, office, and email) was taken directly from the current live
site, so nothing there should need changing.

## Customizing the look

- Colors and fonts are CSS variables at the top of `css/style.css`
  (`--accent` is the oxblood color used for links/tags — change it there to
  re-theme the whole site).
- Dark mode follows the visitor's OS setting automatically (see the
  `prefers-color-scheme: dark` block in the CSS).
