# NEXORA Technologies V13 — Deployment & Security Maintenance

Based on V12 Modular; original `logo.png`, UI, bilingual features, project cards, contact form, and 3D effects preserved.

## Fixed
- Canonical, Open Graph, Twitter image, JSON-LD Organization URL and project Visit website link now point to https://mapdllah306.github.io/nexora-technologies/.
- robots.txt and sitemap.xml now use the correct GitHub Pages project path.
- Admin page marked noindex; local editor stays separate from the public deployment.

## Publish to GitHub Pages
Upload `index.html`, `logo.png`, `content.json`, `robots.txt`, `sitemap.xml`, `.nojekyll`, the `css/` folder's `style.css`, and the `js/` folder's `main.js`, keeping folder structure. **Do not upload** `admin.html`, `js/admin.js`, `css/admin.css`, or ADMIN_SECURITY.md if the editor must remain local.

The ZIP includes the local editor for your personal use. GitHub Pages cannot provide authenticated admin controls without a separate backend/auth service. See ADMIN_SECURITY.md.

## Checks
JavaScript syntax, JSON parse, XML parse, relative references and ZIP integrity verified offline. Browser behavior and live deployment require post-publish testing.
