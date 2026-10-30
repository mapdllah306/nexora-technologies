# NEXORA V21 — Founder Card Critical Fix

## Confirmed root cause
V20 shipped `css/founder.css` but `index.html` did not link to it. This made the founder modal appear unstyled and caused severe mobile layout overflow. V21 explicitly loads `css/founder.css?v=21` after `css/style.css?v=21`, and includes refined founder capsule styling and constrained mobile dialog sizing.

## Publish
Upload `index.html`, the **entire** `css/` and `js/` folders, `founder-portrait.webp`, `logo.png`, `content.json`, `robots.txt`, `sitemap.xml`, `.nojekyll`. Do not upload admin files to the public site if you want to keep the local editor private.

## Verification
Static reference and syntax checks passed; actual mobile browser rendering still requires live testing.
