---
name: website-vibecoding
description: Use when building, editing, or deploying the jc.riv-website artist portfolio. Covers HTML/CSS templates, series/course creation, GitHub Pages deployment, and vibe coding workflows for static sites.
---

# jc.riv-website — Vibe Coding Skill

This skill guides the AI to build a clean static artist portfolio using raw HTML + CSS.

## Template System

### Adding a new Art Series
1. Copy `series/series-template.html` → `series/series-<name>.html`
2. Replace the 3 marked `<!-- CHANGE: -->` sections: `<title>`, hero `<h1>`, and gallery `<img>` tags
3. Add `<li><a href="series/series-<name>.html">Name</a></li>` to the nav in `index.html`

### Adding a new Course
1. Copy a `<div class="course-card">...</div>` block in `courses/index.html`
2. Edit the title, description, date, and link inside the copy

## CSS Rules
- All custom properties in `:root` inside `styles.css`
- Mobile-first: write base styles for mobile, wrap desktop overrides in `@media (min-width: 768px)`
- Images: use `max-width: 100%; height: auto;`

## Deployment
`git add -A && git commit -m "..." && git push`
