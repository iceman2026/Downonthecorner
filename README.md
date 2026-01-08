# Downonthecorner

Tiny demo repository with a small static Unsplash demo and HTML validation CI.

Quick start

- Open `index.html` in a browser to view the Unsplash demo (random images).
- Install dev tools: `npm install` (requires Node.js)
- Run local HTML validation: `npm test` (uses `html-validate`)

Features added in this repository

- `index.html` — Unsplash demo with a client-side ALDATA URL input
- `package.json` — minimal dev dependency (`html-validate`) and `test` script
- `.github/workflows/ci.yml` — runs the HTML validation on push and pull requests
- `.github/copilot-instructions.md` — guidance for AI agents and contributors

Notes

- Do not commit local virtual environments; `.venv` is ignored via `.gitignore`.
- If your company uses an internal image service (e.g., "alldata"), use the ALDATA URL field in the demo to load images from that provider (no auth required for direct image URLs).

Contributing

Please open a PR for non-trivial changes — CI will validate HTML on every push/PR.