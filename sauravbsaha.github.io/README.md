# sauravbsaha.github.io

Personal academic and professional website for **Saurav Bhaskar Saha, PhD, FRSB** —
Senior Scientist, Bioinformatics at Sygnature Discovery.

Live at <https://sauravbsaha.github.io/>

## Structure

| Path | Purpose |
| --- | --- |
| `index.html` | The entire site — a single self-contained page (HTML, CSS and JS inline). |
| `404.html` | Styled not-found page served by GitHub Pages. |
| `images/profile.jpg` | Portrait used in the hero and as the social-share image. |
| `robots.txt`, `sitemap.xml` | Search-engine hints. |
| `.nojekyll` | Serves files as-is; skips Jekyll processing. |
| `assets/` | Unused leftovers from an earlier HTML5 UP template. Safe to delete. |

There is no build step and no external dependency: no CDN, no framework, no
web fonts. The page works offline and renders from a single file.

## Editing

Open `index.html` and edit the relevant `<section>`. Sections are marked with
comment banners (`<!-- ============ EXPERIENCE ============ -->`).

Common edits:

- **Text and dates** — edit the section markup directly.
- **Colours** — change the CSS custom properties in the `:root` block near the
  top of the `<style>` element. Dark-mode overrides live in the matching
  `@media (prefers-color-scheme: dark)` and `:root[data-theme="dark"]` blocks.
- **Portrait** — replace `images/profile.jpg` (a square image works best; the
  hero crops it to a circle).
- **Navigation** — add a section with an `id`, then add a matching
  `<a href="#id">` inside `<nav class="nav-links">`. The scroll-spy highlight
  picks it up automatically.

## Preview locally

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Publish

GitHub Pages serves the `master` branch of this repository. Commit and push:

```bash
git add -A
git commit -m "Update site"
git push origin master
```

Changes are usually live within a minute.

## Notes

- The site is responsive, keyboard-navigable, and supports light and dark themes
  (following the operating-system preference, with a manual toggle that is
  remembered per browser).
- A print stylesheet is included, so **Print → Save as PDF** produces a clean,
  CV-style document from the page.
- The email address is assembled in JavaScript rather than written into the
  markup, which deters naive address harvesters. Visitors without JavaScript
  still see a readable `name [at] domain` form.
