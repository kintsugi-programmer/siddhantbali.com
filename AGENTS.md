# AGENTS.md

## What this repo is

Personal resume website. The **entire site is a single static file: `index.html`** — no build step, no dependencies, no dev server, no tests, no lint config. Preview by opening `index.html` in a browser.

## Critical: two sources of truth

`resume.tex` (Jake Gutierrez / sb2nov LaTeX template) and `index.html` (hand-ported HTML/CSS replica of that resume) contain the **same resume content**. They are kept in sync manually.

- If you edit resume content (jobs, projects, skills, links, contact info), **update both files**.
- `resume.tex` also contains many commented-out draft entries — that's intentional scratch space; don't "clean it up" unless asked.

## Conventions

- External links use `target="_blank" rel="noopener"` in `index.html` — preserve this on any new link.
- `index.html` styling is intentionally a faithful clone of the sb2nov LaTeX resume look (11pt Helvetica, 8.5in page, section rules). Avoid restyling unless asked.
- Special characters in HTML use entities (`&rsquo;`, `&ndash;`, `&amp;`); LaTeX uses its own escapes (`\&`, `--`, `$|$`). Match each file's convention.
- Deployed content comes from `index.html` on `main`; there is no build pipeline to regenerate anything.
