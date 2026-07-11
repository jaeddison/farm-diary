# Farm Diary

A searchable, mobile-first farm logbook for Driffield Farming Ltd — production, herd flags, weather, grazing, and k-line management, all in one tap-to-enter tool. Separate from Dairy Assistant, which handles live herd operations; Farm Diary is the historical record you scroll back through.

Built as a single self-contained HTML file. No backend, no build step, no account — all data is stored locally in your phone's browser via `localStorage`.

## Setup (GitHub Pages)

1. Create a new repository on GitHub — e.g. `farm-diary`.
2. Upload two files to the repository root:
   - `index.html` (the app itself)
   - `icon.png` (the home screen icon)
3. In the repo, go to **Settings → Pages**.
4. Under **Branch**, select `main` (or `master`) and folder `/ (root)`, then **Save**.
5. GitHub will publish the site at:
   `https://<your-github-username>.github.io/farm-diary/`
   (This can take a minute or two on the first publish.)

## Add to iPhone home screen

1. Open the GitHub Pages link above in **Safari** (not Edge — Apple only allows "Add to Home Screen" with a custom icon from Safari).
2. Tap the **Share** button, then **Add to Home Screen**.
3. You'll see the green "FD" icon and the name **Farm Diary** — tap **Add**.

Once added, it opens full-screen like a native app, with no browser address bar.

> If you've already added it once without the icon, remove the old home screen shortcut and re-add it after uploading `icon.png`, otherwise iOS will keep the old screenshot-style icon.

## Data & backups

All entries live in your phone's browser storage. That means:

- Data stays on your phone — nothing is sent anywhere.
- Clearing Safari's site data/history for this page will erase it, so avoid "Clear website data" for this address.
- Use the **Export** section in the History tab to pull a date range out as a text block (production, k-line, or grazing) any time you want a backup or want to hand data off for further analysis.

## Structure

- **Today** — date-selectable entry: Production, Trends, Herds & Flags, Weather, Grazing, Notes
- **K-line** — Pod 1 and Pod 3 paddock tracking with a running consecutive-days counter
- **History** — searchable log with a rainfall/production heatmap and the Export tool

## Updating the app

When a new version is built, just re-upload the updated `index.html` to the same repository (overwrite the existing file) and GitHub Pages will publish the change automatically — your saved data isn't affected, since it lives in the browser, not in the file.
