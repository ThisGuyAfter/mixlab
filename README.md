# MixLab - Signal Flow Reference

A mobile-first Progressive Web App (PWA) for instrument-by-instrument mixing chains.

## Files
- `index.html`: complete app and reference content
- `manifest.webmanifest`: Home Screen app metadata
- `sw.js`: offline caching
- `icon-192.png`, `icon-512.png`: app icons

## Deploy (free option: GitHub Pages)
1. Create a GitHub repository (for example, `mixlab`).
2. Upload all five files in this folder to the repository root.
3. In the repository, open Settings -> Pages.
4. Under Build and deployment, choose Deploy from a branch, select `main` and `/ (root)`, then Save.
5. Wait for GitHub Pages to publish the site. Open the HTTPS URL on your iPhone in Safari.
6. Tap Share -> Add to Home Screen -> Add.

The app caches its core files after the first successful visit. Favorites and notes are stored locally in the browser on that device.

## Notes
- HTTPS hosting is required for service workers and normal PWA installation.
- The app does not require an account or send notes/favorites to a server.
- To update the app after editing files, change the cache version in `sw.js` (for example, `mixlab-v2`).
