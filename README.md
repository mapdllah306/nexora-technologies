# NEXORA Technologies V6 — Immersive 3D

This release extends V5 without replacing its logo, content, language/theme switchers, projects or contact details.

## Changes
- Optional WebGL GPU particle field in the hero; original Canvas 2D fallback retained.
- 30fps visual throttling and reduced particle count on mobile.
- Pauses offscreen or in background; respects reduced-motion preferences.
- Escape and outside-click close the mobile menu.

## GitHub Pages
Upload `index.html` and `logo.png` to the same repository root, replacing V5 files. No build tools or external JavaScript libraries needed.

## Note
WebGL is a true GPU-rendered particle layer, not a 3D model or 3D reconstruction of the logo. The original logo image is preserved.
