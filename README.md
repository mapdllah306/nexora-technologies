# NEXORA Technologies V7 — Quality & Stability

Based directly on V6. The original logo, bilingual copy, sections, contact links, theme switcher and WebGL effects are preserved.

## Audit and changes
- Prevented the Canvas 2D animation from continuing behind WebGL, and restarted it on WebGL context loss.
- Protected language/theme preferences from localStorage access errors.
- Improved small-screen card density, wrapping and tap targets.
- Made closed mobile navigation inert for keyboard/screen-reader navigation.
- Added vertex shader precision for WebGL 1 portability.
- Added logo intrinsic dimensions and high-priority loading.
- Improved reduced-motion CSS and visibility detection.

## Publishing
Upload index.html and logo.png to the root of the existing GitHub Pages repository. Keep a copy of V6 for rollback.

## Validation
Syntax and archive checks run locally. Browser/device testing remains necessary, particularly Android WebGL and screen readers.
