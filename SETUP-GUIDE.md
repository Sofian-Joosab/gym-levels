# Gym Levels PWA — Setup Guide

## Easiest: Host free on GitHub Pages (5 minutes)

1. Go to **github.com** → click **+** → **New repository**
2. Name it `gym-levels`, set it to **Public**, click **Create**
3. Click **"uploading an existing file"** link
4. Unzip `gym-levels-pwa.zip` and drag ALL files/folders in:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icons/` folder (with both PNGs)
5. Click **Commit changes**
6. Go to **Settings** → **Pages** → Source: **main** branch → **Save**
7. Your app will be live at: `https://YOUR-USERNAME.github.io/gym-levels/`

## Install on your Android phone

1. Open the URL in **Chrome** on your phone
2. You'll see a banner **"Add Gym Levels to Home screen"** — tap it
3. If no banner appears: tap the **⋮ menu** → **"Install app"** or **"Add to Home screen"**
4. The app icon will appear on your home screen
5. It runs fullscreen like a native app, works offline after first load

## Alternative: Host locally (for testing)

If you have Python installed on your PC:

```bash
cd gym-levels-pwa
python3 -m http.server 8080
```

Then open `http://localhost:8080` in Chrome. Note: PWA install requires HTTPS,
so local testing won't trigger the install prompt (but the app works fine).

## Alternative: Host on Netlify (also free)

1. Go to **app.netlify.com**
2. Drag the unzipped folder onto the page
3. Done — you get a URL like `random-name.netlify.app`
4. Open that URL on your phone and install as above

## Your data

All workout data, XP, and progress is saved in your phone's browser storage.
It persists between sessions. Clearing browser data will reset your progress.
