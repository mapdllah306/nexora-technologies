# NEXORA Technologies V9 — Business Inquiry Edition

## Previous-version audit
- Reviewed V8 portfolio markup, filter logic, modal translation, contact section, and responsive rules.
- Existing V8 contact link opened an empty email draft; no structured project intake existed.
- GitHub Pages is static: it cannot securely receive or store form submissions without a backend or external service.
- The V8 code still contains a separate portfolio translation dictionary; retained it to avoid regression, with further consolidation recommended.

## Changes
- Added bilingual project inquiry form with name, email, service, optional budget and timeline, and project details.
- Uses browser validation and explicit user consent.
- Generates a mailto draft; **it does not submit or store data**. The visitor must send the email from their email app.
- Provides WhatsApp as a fallback, preserves existing contact links and portfolio.
- Responsive form, keyboard focus indicators, and live status text.

## Security and privacy
- No API keys, no server-side storage, no third-party form endpoint, no analytics added.
- Form content is passed to the visitor's configured email application through a mailto URL. It may be visible in browser history or OS handlers. Do not enter sensitive financial or identity information.
- Browser/device must have an email handler; otherwise users can use existing email or WhatsApp links.
- For automatic submission in a future release, deploy a real backend with server-side validation, spam prevention, privacy notice, and secure notification delivery.

## Checks
- JavaScript syntax checked with Node.js.
- HTML structural elements and archive integrity checked programmatically.
- Browser visual and end-to-end email-handler tests are not claimed.

## Deploy
Upload index.html and logo.png to the root of your GitHub Pages repository, replacing the previous versions. Keep a backup of V8.
