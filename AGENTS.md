# AGENTS.md

## Cursor Cloud specific instructions

This is a static HTML/CSS/JavaScript website (no build step, no package manager, no dependencies).

### Running the dev server

Serve the site from the repository root using Python's built-in HTTP server:

```bash
python3 -m http.server 8080
```

The site is then available at `http://localhost:8080`.

### Key files

- `index.html` — single-page site entry point
- `assets/css/style.css` — all styles
- `assets/js/script.js` — navbar toggle, sticky header, search box, scroll animation
- `assets/images/` — static image assets

### Notes

- No linting, testing, or build tooling is configured in the repo.
- External CDN resources (Ionicons, Google Fonts) require internet access; the site renders without them but icons and custom fonts will be missing.
- The GitHub Actions workflow (`.github/workflows/static.yml`) deploys to GitHub Pages; it is not needed for local development.
