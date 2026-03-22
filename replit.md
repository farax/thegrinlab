# Grin Lab — Innovation. Not Complicity.

## Project Overview

A single-page static marketing website for **Grin Lab** (`www.thegrinlab.com`). The site is entirely self-contained in a single `index.html` file with all CSS and JavaScript inline.

## Architecture

- **Type:** Static HTML site (no build system, no package manager, no backend)
- **Entry point:** `index.html` (1716 lines, all-in-one)
- **Fonts:** Google Fonts (Cormorant Garamond, Jost, Space Mono, DM Sans, DM Mono, Instrument Serif)
- **No external dependencies** beyond Google Fonts CDN

## Development Server

Served via Python's built-in HTTP server:

```
python3 -m http.server 5000 --bind 0.0.0.0
```

- **Workflow:** "Start application" — runs automatically on port 5000
- **Output type:** webview (port 5000)

## Deployment

- **Target:** Static site deployment
- **Public directory:** `.` (root, serves `index.html` directly)
- **Custom domain:** `www.thegrinlab.com` (configured via `CNAME` file)

## File Structure

```
/
├── index.html      # Entire site — HTML, CSS, JS all inline
├── CNAME           # Custom domain: www.thegrinlab.com
└── replit.md       # This file
```
