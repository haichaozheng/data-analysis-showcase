# AGENTS.md

## Stack

Pure static HTML + CSS. No build step, no JS framework, no package.json. Push to `main` deploys via GitHub Pages.

## Local preview

```
python -m http.server 8000
```

Then open http://localhost:8000/index.html

## Critical convention: nav & footer are copy-pasted

`<nav>...</nav>` and `<footer>...</footer>` are duplicated in every HTML file. Changing either requires updating **all** HTML files in sync:

- `index.html`, `intro.html`, `timeline.html`, `rules.html`, `projects.html`, `resources.html`, `news.html`

## Adding content

- **New project card** (`projects.html`): copy the template in README.md. Badge classes: `badge-progress` (yellow), `badge-live` (green), `badge-demo` (orange).
- **New news item** (`news.html`): copy the comment template already inside `news.html`, place at top of `.news-list`.

## Language

All content is `zh-CN`. Do not add English-only text.
