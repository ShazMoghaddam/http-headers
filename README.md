# HTTP Headers, Decoded

A searchable field guide to the headers browsers and servers attach to every HTTP request and response, grouped by role with a plain-English meaning for each. One self-contained HTML page, no build step.

**Live:** https://shazmoghaddam.github.io/http-headers/

## What it does

- Search every header by name or meaning, with the matching text highlighted in the results
- Filter by role, with shareable per-category links (for example `.../#security` for the security headers)
- An "Essential headers" filter for the ones you actually set day to day
- Keyboard: press `/` to jump to search, `Esc` to clear it
- Share button (uses the native share sheet, or copies the link) and Save as PDF
- Colour-coded classes and a link-preview card for social posts

## What's inside

61 headers across 7 classes:

- **Request** — what the client tells the server (Host, Accept, Authorization, Cookie)
- **Response** — what the server tells the client (Location, Set-Cookie, Retry-After)
- **Content & encoding** — how the body is described (Content-Type, Content-Encoding)
- **Caching** — how responses are stored and reused (Cache-Control, ETag, Vary)
- **Conditional & range** — asking for part, or only if changed (If-None-Match, Range)
- **CORS** — the cross-origin sharing set (Access-Control-Allow-Origin and friends)
- **Security** — hardening the browser (HSTS, CSP, X-Frame-Options, the COOP/COEP/CORP set)

The deprecated headers people still run into (X-XSS-Protection, Expect-CT, Public-Key-Pins, DNT) are included and clearly labelled, so the reference is honest about what to remove as well as what to set.

## Put it live on GitHub Pages

1. Create a new public repo named `http-headers`.
2. Add `index.html` and `preview.png` to the root of the repo.
3. Settings, then Pages. Source: "Deploy from a branch", branch `main`, folder `/ (root)`, Save.
4. Give it a minute, then open https://shazmoghaddam.github.io/http-headers/

If you name the repo something else, update the three absolute URLs near the top of `index.html` (`canonical`, `og:url`, `og:image`).

## Files

- `index.html` — the page
- `preview.png` — the 1200x630 card shown when the link is shared

Made by Shaz Moghaddam.
