# NEXORA V10 — Cinematic 3D Evolution

## Baseline
Based on V9, preserving its original logo, sections, portfolio, bilingual copy, theme switching and inquiry draft workflow.

## Audit and changes
- V9 WebGL had no fully implemented context-restoration pathway. This remains an open issue; fallback is retained.
- Added an explicit bilingual Motion On/Off control, persisted locally when available.
- Added a lightweight animated cinematic halo around the original logo; no replacement assets.
- Motion off hides both WebGL and Canvas layers and stops their animation loops.
- Added live announcement semantics to inquiry form status.
- Kept mobile layout, project dialogs, filters, and mailto behavior.

## Validation
Static code checks only. Browser, GPU context loss/recovery, bilingual interaction, reduced-motion and mobile device testing are required before production acceptance.

## Deployment
Upload index.html and logo.png to the GitHub Pages repository root. Preserve a backup of V9 first.
