# NEXORA V11 — SEO & Global Reach

## Baseline and preservation
Built from V10 `index.html` and the identical original `logo.png`. Existing project gallery, bilingual content, contact form, motion control, WebGL/Canvas and theme settings remain.

## V10 audit and V11 fixes
- Removed duplicated `role` and `aria-live` attributes on the inquiry status element.
- Added canonical URL, robots directive, Open Graph, Twitter/X card, favicon and Organization JSON-LD.
- Added `robots.txt` and `sitemap.xml` for the public GitHub Pages root URL.
- Language-specific page title and description now update when language changes.
- `?lang=ar` and `?lang=en` are recognized as explicit language selection on arrival.

## Important SEO limitations
- This is still one JavaScript-localized URL. We intentionally DO NOT add hreflang alternate links: true language-specific indexed pages require distinct server-delivered localized URLs. Query-language links alone do not guarantee separate search indexing.
- Social platforms generally fetch the initial HTML and will display the default English share metadata, even when the viewer selected Arabic.
- `logo.png` is a square logo, not a custom 1200×630 social banner. Some platforms may crop it.
- Search engine indexing and ranking are not guaranteed. Verify the deployed public URL and submit the sitemap in Google Search Console.
- This package assumes the site is published at `https://apdllah306.github.io/` (repository root). If using a project path or custom domain, change canonical/OG/sitemap URLs before deployment.
- No new analytics, trackers, paid services or external JS dependencies.

## Deployment
Upload ALL FIVE files (`index.html`, `logo.png`, `robots.txt`, `sitemap.xml`, `README.md`) into the GitHub Pages publish root, then commit. README is optional for runtime.

## Verification scope
Static checks: file presence, valid XML and JSON-LD, JavaScript syntax and ZIP integrity. Browser rendering, Lighthouse scores, Google Search Console and real social previews are NOT verified here.
