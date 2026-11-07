# Biology to Beyond — Kathir V.

Static portfolio for GitHub Pages: `index.html` plus assets. No build step, no dependencies.

## Publish
Settings → Pages → Deploy from a branch → `main` and `/(root)`.

## Structure
- `index.html` — page, styles and scripts (inline)
- `kathir-portrait.jpg` — hero portrait
- `assets/resumes/` — one PDF per target role

## Resumes
Four one-page PDFs in `assets/resumes/`: ML Engineer, Data Scientist, Data Analyst, Bioinformatics Analyst.

To add a role, drop a PDF into `assets/resumes/` and add one `<li class="role-row" data-build>` to the `#resumes` list.

## Scroll build effect
Blocks marked `data-build` are placed one at a time as they scroll into view, with two labelled cursors,
a selection box and a short build log. It is one-shot (no scroll-scrubbing), uses only transform and
opacity, and is switched off entirely under `prefers-reduced-motion`.