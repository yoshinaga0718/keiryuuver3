
# Keiryu Inspection PWA

This repo contains a ready-to-deploy Progressive Web App (PWA) for field inspections.

## Files
- `index.html` – App UI (GPS, add/delete rows, export TSV/CSV/KML, etc.)
- `manifest.webmanifest` – PWA manifest
- `sw.js` – Service Worker (offline cache)
- `icons/icon-192.png`, `icons/icon-512.png` – App icons

## Quick Deploy (GitHub Pages)
1. Create a new public repo on GitHub (e.g., `keiryu-inspection`).
2. Upload these files to the **root** of the repo (keep `icons/` folder).
3. Go to **Settings → Pages** → Source: `Deploy from a branch` → Branch: `main` / Folder: `/ (root)` → Save.
4. Open the published URL (e.g., `https://<your-id>.github.io/keiryu-inspection/index.html`).
5. On your phone: **Add to Home Screen** / **Install**. Works offline after first load.

## Update Tips
- If changes don't show up, bump `CACHE_NAME` in `sw.js` (e.g., `-v2`) and reload.
- Manifest/icon paths must remain relative to repo root.
