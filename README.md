# KIVRA — Version 1.0.0

A mobile-first PWA prototype for nutrition tracking, fitness challenges and a community experience.

## What's included
- Arabic / English interface and RTL/LTR switching.
- Dark premium interface with neon-green accents and optional light mode.
- Daily dashboard for calories, protein, carbs and water.
- Searchable starter food list with portion scaling.
- Manual custom-food entry.
- Meal diary saved locally on the device.
- Meal photo selection and preview.
- Challenges, local community posts and profile goals.
- Export/import local backup.
- PWA manifest and service worker.

## Important limitations in this first release
1. **AI photo calorie analysis is not connected yet.** The interface accepts a photo and previews it, but a real analysis requires a secure server endpoint and an AI provider. Do not put private API keys in `app.js` or any browser file.
2. **Community is local-only.** Posts are stored on the current device. Real accounts, cross-device sync, moderation and social features require a backend.
3. **Food values are estimates.** The included food list is a small starter dataset. Portion size, recipe and cooking method change nutrition values. Users can enter custom values.
4. This prototype does not provide medical advice or prescribe calorie goals.

## Run locally
Open `index.html` in a browser for basic testing. For installable PWA behavior and service-worker caching, host the folder on an HTTPS static host (for example GitHub Pages).

## Publish using GitHub Pages
1. Extract the ZIP.
2. In your KIVRA GitHub repository choose **Add file → Upload files**.
3. Upload the contents of this folder (not the outer KIVRA folder) so `index.html` is at the repository root.
4. Commit the upload to the `main` branch.
5. Open **Settings → Pages**.
6. Under Build and deployment choose **Deploy from a branch**, branch `main`, folder `/ (root)`, then Save.
7. Wait for the Pages URL to appear. Open it on Android Chrome and use **Add to Home screen**.

## Before a public launch
- Add secure authentication and a database.
- Connect real AI photo analysis through a server-side endpoint.
- Expand and verify the food database.
- Add privacy policy, terms, deletion/export controls and abuse reporting.
- Test accessibility, security, performance and nutrition accuracy.
