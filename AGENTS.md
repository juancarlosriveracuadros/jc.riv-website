# Project: jc.riv-website — Artist Portfolio

## Overview
Static multi-page website for an artist. Built with raw HTML + CSS, no frameworks. Deployed on GitHub Pages.

## Architecture
- **Landing page** (`index.html`): artist bio + CV timeline + navigation hub
- **Series pages** (`series/`): one `.html` file per art series, copied from `series-template.html`
- **Courses page** (`courses/index.html`): card-based layout, add courses by copying a card snippet
- **Global styles** (`styles.css`): CSS custom properties, reset, nav, footer — shared across all pages
- **Images**: `assets/images/<series-name>/` — group by series

## Conventions
- Every new series = copy `series-template.html`, rename, swap content in the 3 marked spots
- Every new course = copy a `<div class="course-card">` block into `courses/index.html`
- Prefer semantic HTML5 (`<nav>`, `<main>`, `<section>`, `<article>`, `<figure>`)
- CSS uses custom properties for colors/spacing (defined in `styles.css`)
- Mobile-first responsive design
- Images stay under 500 KB each

## Vibe Coding Workflow
1. AI writes/edits files directly
2. User previews in browser (open `index.html` locally)
3. Changes committed and pushed to GitHub Pages
4. New series/course = copy template, edit data, add nav link, commit

## Tech Stack
- HTML5, CSS3 (Flexbox, Grid, Custom Properties)
- Google Fonts (Inter + Merriweather)
- Git + GitHub Pages for hosting
- No build tools, no JavaScript frameworks, no backend
