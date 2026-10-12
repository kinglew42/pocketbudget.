# PocketBudget — iPhone install package

## Files
- `index.html`: the app
- `manifest.json`: install name, icon, and standalone display settings
- `sw.js`: caches the app shell for offline opening after the first online visit
- `icon-192.png`, `icon-512.png`: app icons

## Publish free with GitHub Pages
1. Create or sign in to a GitHub account.
2. Create a **public** repository named `pocketbudget` (or any name).
3. Upload all files from this folder to the repository's root (not the ZIP itself).
4. Open repository **Settings → Pages**.
5. Under build/deployment, choose **Deploy from a branch**, select `main` and `/ (root)`, then Save.
6. Wait for GitHub Pages to publish the site. Its URL will look like `https://YOUR-USERNAME.github.io/pocketbudget/`.
7. Open that URL in **Safari** on your iPhone. Tap **Share → Add to Home Screen**. If shown, enable **Open as Web App**, then tap **Add**.

## Important data note
This version stores its budget data in local storage on the device/browser where you use it. It does not sync across devices. Use **Backup** regularly to download a JSON backup, and use Settings → Restore backup to restore it. Avoid clearing Safari website data unless you have a backup.

Scheduled paychecks are added when the app is opened on or after their due date; they do not run in the background while the app is closed. Pay estimates are simplified and do not account for taxes, overtime, or employer payroll rules.

## Privacy
There is no bank connection, login, analytics, or external database in the app. GitHub Pages hosts the static app files; your budget entries are not uploaded to GitHub by using the app.
