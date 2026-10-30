# NEXORA Technologies V14 — Deep Audit & Experience Polish

## Scope
Based on the complete local V13 package. All original logo, layout, portfolio, forms, bilingual copy, animations and static content management preserved.

## Changes
- Moved cinematic motion switch from crowded navigation into a compact Settings popover. Persists preference, respects OS reduced motion by default, supports Arabic/English, keyboard Escape and click-away.
- Added bilingual NEXORA website assistant in a discreet floating panel, with local intent matching and suggested questions. **This is not a generative AI model**; it makes no remote calls and uses no API key. A real LLM assistant requires a secure backend, provider and budget.
- Extracted assistant code into `js/assistant.js` and styling into existing `css/style.css`; modular architecture retained.
- Reviewed original links, metadata, JSON content, project dialogs, motion handling, contact form, admin separation and GitHub Pages paths.

## Deployment
Upload `index.html`, `logo.png`, `content.json`, `.nojekyll`, `robots.txt`, `sitemap.xml`, `css/` and `js/` to the repo root. Keep `admin.html`, `css/admin.css`, `js/admin.js`, `ADMIN_SECURITY.md` private/local.

## Test limits
Static syntax/structure/archive tests performed; live interactive mobile/browser validation remains necessary. No claim of comprehensive security penetration testing or real AI integration.


## V15 — Robot Assistant Experience
- Animated CSS robot head inside the assistant launch button, with illuminated interactive face and talking mouth.
- Progressive grapheme-aware typewriter effect for bot replies.
- Optional speech synthesis with language-specific voices (Arabic Egypt / English US), stop button and mute checkbox. Browser voice availability and autoplay policies vary; voice may require user interaction or an installed Arabic voice. Mouth motion approximates speech activity, not phoneme-accurate lip sync.
- Honors reduced-motion preference; cancels pending speech and typing when a new question is submitted or the panel closes.
- No external API, microphone access, secret keys, or network requests introduced. Local rule-based assistant remains unchanged.
- Test on real Android browsers before production sign-off.
