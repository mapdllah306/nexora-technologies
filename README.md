# NEXORA Technologies V17 — Mobile Robot UI Repair

Based on V16. Preserves site content, logo, separate CSS/JS, assistant local answers, text animation and browser speech synthesis.

## Fixes
- Fixes root cause of chat overlay: V16 set `data-open` on the dock wrapper but the CSS targeted the assistant container. V17 correctly sets the state on `#nxAssistant`.
- Uses a viewport-bounded fixed chat panel with scroll confined to the messages area, mobile safe-area spacing, and constrained bubble widths.
- Moves the same robot head between the collapsed launcher and expanded chat header, rather than rendering two robots.
- Reduces capsule width and robot size.
- Maintains RTL/LTR behavior.

## Verification
JavaScript syntax, local references, JSON/XML and ZIP integrity checked offline. Visual/browser and voice behavior must be tested after publishing on real devices.

## Publishing
Upload public files including `css/`, `js/`, `index.html`, `logo.png`, `content.json`, `robots.txt`, `sitemap.xml`, `.nojekyll`. Keep `admin.html`, `css/admin.css`, `js/admin.js`, `ADMIN_SECURITY.md` private unless you deliberately want a publicly accessible editor.


## V18 — Robot Head Above Chat
- The robot stage is moved to the assistant root while the chat is open, and back into the capsule dock when closed.
- The robot remains visible above the chat panel without clipping or overlapping messages.
- Speech, typing animation, localization and existing website modules remain unchanged.
- Static checks completed; browser/device verification still required.
