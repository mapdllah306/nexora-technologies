# NEXORA V12 — Modular Source Edition

Refactor of V12 with separate HTML, CSS and JavaScript. No new backend or login is introduced.

## Files
- `index.html`: public site markup and SEO structured data (JSON-LD)
- `css/style.css`: public site styling
- `js/main.js`: public site logic, translations, WebGL and contact interactions
- `admin.html`: local editor markup
- `css/admin.css`: local editor styling
- `js/admin.js`: local editor behavior
- `content.json`: editable bilingual content
- `logo.png`: unchanged original brand image
- `robots.txt`, `sitemap.xml`: search engine metadata

## Deployment
Upload `index.html`, `css/`, `js/`, `content.json`, `logo.png`, `robots.txt`, and `sitemap.xml` to the GitHub Pages repository, preserving paths. The `admin.html` editor is intended for local use only and is not password protected.

Open the public site through a web server / GitHub Pages; `fetch('content.json')` may fail when opening via `file://`.

## Verification
Syntax checks performed for JavaScript, JSON and XML. This is a structural refactor, not a browser regression test.
