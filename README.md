# Stride — Android installable PWA

Upload these six files directly to the root of your GitHub Pages repository:
`index.html`, `manifest.json`, `service-worker.js`, `icon-192.png`, `icon-512.png`, and `README.md`.

## Install on Android
1. In your existing GitHub repository, replace the old `index.html`, `manifest.json`, and `service-worker.js` with these versions.
2. Upload `icon-192.png` and `icon-512.png` to the repository root (same level as `index.html`). Keep `README.md` if you like.
3. Wait 1–3 minutes for GitHub Pages to update.
4. On Android Chrome, open the published website. Refresh it once or twice.
5. If Chrome still says it cannot be installed, clear that website's stored data in Chrome settings or open the URL in an Incognito tab only to test; then return to the normal tab and try Chrome menu → Install app / Add to Home screen.

## Notes
- The app shell and icons are now all at the repository root, avoiding missing nested icon paths. The page registers the service worker, which caches the app for offline use after the first successful online load.
- Daily reminders can only fire reliably while the Stride page is open. Android may suspend JavaScript when the app is closed; reliable closed-app reminders need push notifications or a native Android app.
- Your habit data remains on that device in browser storage; it is not synced to an account.
