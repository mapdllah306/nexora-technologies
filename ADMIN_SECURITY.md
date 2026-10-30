# NEXORA V13 — Secure Publishing Workflow

The website is hosted on GitHub Pages, which serves public static files. `admin.html` is a local-only content editor, **not an authenticated admin dashboard**. Do not upload `admin.html` to the public repository.

## Publishing content safely
1. Keep `admin.html`, `js/admin.js` and `css/admin.css` locally (do not publish them). Open the editor on your own device using a local web server if the browser blocks local files.
2. Export the generated `content.json` and inspect it. Never include passwords, access tokens, private customer information or credentials.
3. Sign in to GitHub yourself using a passkey or strong password and two-factor authentication.
4. In the `nexora-technologies` repository, edit/upload `content.json` using GitHub's authenticated interface. Commit the changes. GitHub Pages will deploy them.
5. For changes to layout or behavior, edit `css/style.css`, `js/main.js` and `index.html` separately.

## Why no password box?
Client-side JavaScript and HTML cannot safely keep an admin password or GitHub token secret. A truly remote admin dashboard requires an authentication provider and a backend with authorization, validation and audit logging.

## Recommended repository protections
Enable 2FA for GitHub, restrict collaborator access, review commits, and optionally require pull requests on the production branch. Do not commit secrets.
