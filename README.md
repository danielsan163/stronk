# Stronk

A personal workout log that runs in Safari on your iPhone. Your log is saved on the phone only, so export a backup now and then.

## Put it on GitHub Pages

1. On github.com, create a new repository named `stronk`. Public is fine: the code is public, but your workout data never leaves your phone. GitHub Pages on a private repo needs a paid plan.
2. Push this folder to it:
   ```bash
   git init -b main
   git add .
   git commit -m "Stronk"
   git remote add origin https://github.com/YOUR-USERNAME/stronk.git
   git push -u origin main
   ```
3. In the repo, go to **Settings → Pages**, set Source to **Deploy from a branch**, and pick `main` and `/ (root)`. Save.
4. After a minute or so it's live at `https://YOUR-USERNAME.github.io/stronk/`.

## Add it to your iPhone

1. Open that address in **Safari** (not a Private tab).
2. Tap **Share → Add to Home Screen**.
3. Always open Stronk from the Home Screen icon. That copy keeps its storage most reliably, and it works with no signal once you've opened it once.

## Backups

On the Workout tab, under **Your data**:
- **Export backup** opens the share sheet. Choose **Save to Files** and put it in iCloud Drive.
- **Import backup** reads a backup file and merges it in. Use it on a new phone or after clearing Safari.

The app nudges you once 14 days have passed since your last backup.

## Updating the app

After changing `index.html`, bump `VERSION` in `sw.js` (for example `stronk-v2`) and push. Phones pick up the new copy the next time they open it with a signal.
