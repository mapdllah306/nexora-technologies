# NEXORA V20 — Founder Card Repair

V19 mobile screenshot exposed a catastrophic unstyled modal / desktop-scaled layout. This patch isolates founder styles in `css/founder.css` and version-busts CSS and founder JS URLs to avoid old GitHub Pages browser caches. Includes viewport hardening and fixes a ResizeObserver lifecycle bug. Preserves portrait and existing site functionality.

## Publish
Upload **all** public files and folders, including new `css/founder.css`. Do not publish `admin.html`, `css/admin.css`, `js/admin.js`, or `ADMIN_SECURITY.md` if you want the local editor private.

## Verification
Static syntax, file references and ZIP tested. Real browser visual test unavailable due to restricted browser networking; user must verify on Android. No claim of pixel-perfect equivalence to the reference image.
