# AGENTS.md

## What this repo is

Personal resume website. The **entire site is a single static file: `index.html`** — no build step, no dependencies, no dev server, no tests, no lint config. Preview by opening `index.html` in a browser.

## Single source of truth

`index.html` is the **single source of truth for all resume content**. The original `resume.tex` (Jake Gutierrez / sb2nov LaTeX template) was removed in commit `47ac115` — the old LaTeX content and its commented-out draft entries remain recoverable from git history if ever needed.

- Edit resume content (jobs, projects, skills, blogs, videos, links, contact info) directly in `index.html`.

## Conventions

- External links use `target="_blank" rel="noopener"` in `index.html` — preserve this on any new link.
- `index.html` styling is intentionally a faithful clone of the sb2nov LaTeX resume look (11pt Helvetica, 8.5in page, section rules). Avoid restyling unless asked.
- Special characters in HTML use entities (`&rsquo;`, `&ndash;`, `&amp;`) — match this in any new content.
- Deployed content comes from `index.html` on `main`; there is no build pipeline to regenerate anything.
