# NEXORA V12 — Content Control Studio

## Audit of V11 and preservation
- V11 contains a single-page bilingual site with CSS/WebGL, contact mailto workflow, portfolio, SEO metadata and light/dark theme. These remain in `index.html` with original `logo.png` unchanged.
- V11 has no backend and cannot securely authenticate administrators or persist edits globally. V12 deliberately does NOT pretend to offer a secure server-side CMS.
- The V11 portfolio translations overwrite project summaries on language switch; V12 reapplies published overrides after the language event.
- Missing `content.json` or network failures leave V11 copy in place. All content overrides use `textContent`, not HTML, to avoid injecting executable markup.

## V12 features
- `admin.html`: local bilingual content editor for nine text fields; JSON import, validation, reset and download.
- `content.json`: publishable public text configuration. Edit locally and upload to the same GitHub Pages root.
- `index.html`: loads `content.json` with graceful fallback. No external services or passwords.

## How to publish
Upload `index.html`, `logo.png`, `content.json`, `robots.txt`, `sitemap.xml` to the GitHub Pages publishing root. Keep `admin.html` OFF the public repository if you want the editing interface to remain local (it is not authenticated, though it cannot write to GitHub).

## Important limits
- This is not a secure online admin panel. It does not manage customer inquiries or remotely update the site. For secure multi-user editing, a server-backed authenticated CMS is required.
- V11's `mailto:` form still requires the visitor to send the message in their email app.
- Edits to headings may not update SEO meta descriptions or the dialog's long project descriptions. Those remain as V11 defaults.
- Browser visual and performance tests are not claimed; test on real devices before deployment.
