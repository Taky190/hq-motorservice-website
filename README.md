# HQ Motorservice website

This is a no-cost static website designed for Cloudflare Pages. It includes Italian and English content, mobile layouts, service pages, editable placeholders, and analytics-ready click events.

## Before publishing

In `assets/app.js`, replace every `#..._URL`, `PHONE_PLACEHOLDER`, `EMAIL_PLACEHOLDER`, and `OPENING_HOURS_PLACEHOLDER` value in the `CONFIG` object. Replace the SVG image placeholders in `assets/` with real HQ images. Add only genuine Google reviews after permission is received.

## Run locally

Install Node.js, then run:

```text
npm run dev
```

Open `http://localhost:3000/it` or `http://localhost:3000/en`.

## Free Cloudflare Pages publishing

1. Create a GitHub repository and upload these files.
2. In Cloudflare, select Workers & Pages, then Create application, then Pages, then Connect to Git.
3. Select this repository.
4. Set the build command to `exit 0` and the output directory to `.`.
5. Deploy.

Cloudflare will serve the internal locale and service routes through `_redirects`.
