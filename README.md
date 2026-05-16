# Events On Main — Static Site

This repository contains the static website for Events On Main.

## Overview

- Primary file: `index.html` (single-page site).
- Assets are under `assets/` (images, favicon, etc.).
- Status: static HTML site — no build step required.

## Quick start (view locally)

Open the site in your browser directly (double-click `index.html`) or run a simple local web server from the repo root (recommended):

```bash
# from the repository root
cd "/Users/djones/Desktop/EventsOnMainSiteFiles"
# Python 3
python3 -m http.server 8000
# then open http://localhost:8000 in your browser
```

## Repository notes

- The footer year is updated automatically at runtime by a small inline script in `index.html`. The script finds the first 4-digit year (e.g. `2025`) inside the `footer` element and replaces it with the visitor's current year. No build step required.

- macOS `.DS_Store` files are ignored. If you see `.DS_Store` in the repo, they have been removed and `.gitignore` updated to contain `.DS_Store`.

## Editing

- Make content edits directly in `index.html`.
- Replace or add images inside `assets/images/` and update references in `index.html`.

## Deployment

This is a standard static site and can be hosted on any static hosting provider (GitHub Pages, Netlify, Vercel static, S3/CloudFront, etc.).

Tips:
- For GitHub Pages, push the `master` (or `main`) branch and enable Pages for the repo.
- For Netlify, drag-and-drop the site folder or connect the repo and publish (no build command).

## Git

Commit and push as usual:

```bash
git add -A
git commit -m "Your message"
git push origin master
```

If you want to avoid automatic commit identity messages on this machine, configure your global git name/email:

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

## License & Contact

Add your preferred license and contact information here (e.g., `LICENSE` file or contact email).

---

If you'd like, I can also:
- Add a small build step (e.g., include a `package.json` and a `npm` script) if you want tooling.
- Create a `LICENSE` file or an `htaccess.example` template for server rules.

