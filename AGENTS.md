# AGENTS.md

## Cursor Cloud specific instructions

This repository is a **static HTML personal website** (`timssweeney.com`, deployed via GitHub Pages). It is hand-written HTML/CSS with no framework, and the entire site is a single page: `index.html` plus assets in `css/`, `fonts/`, and `images/`.

- **No dependencies, no package manager, no build step, no tests, no linters.** There is nothing to install; `python3` (preinstalled) is all that is needed to serve the site locally.
- **Run it (dev):** from the repo root, serve the static files with `python3 -m http.server 8000` and open `http://localhost:8000/`. Opening `index.html` directly also works, but serving avoids relative-path/font issues.
- **Lint / test / build:** none exist. Deployment is simply pushing the static files (GitHub Pages serves `master`).
- External resources (Google Fonts, Font Awesome CDN) are loaded from CDNs; a local Font Awesome copy is also bundled in `css/` + `fonts/`, so the site renders fine offline.
