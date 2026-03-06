# Street Medicine App â€” Deployment Guide

A Progressive Web App (PWA) for documenting street medicine encounters.
Works offline. Installable on iPhone from Safari.

---

## Deploy to iPhone in 5 minutes (GitHub Pages)

### Step 1 â€” Create a GitHub repo

1. Go to https://github.com/new
2. Name it `street-medicine-app` (or anything you like)
3. Set it to **Public**
4. Click **Create repository**

### Step 2 â€” Upload the files

Upload all files from this folder to the repo:
- `index.html`
- `manifest.json`
- `sw.js`
- `icon-192.png`
- `icon-512.png`
- `apple-touch-icon.png`

(Drag-and-drop them directly in the GitHub web interface, or use GitHub Desktop.)

### Step 3 â€” Enable GitHub Pages

1. In your repo, go to **Settings â†’ Pages**
2. Under *Source*, select **Deploy from a branch**
3. Branch: `main` / folder: `/ (root)`
4. Click **Save**
5. Wait ~1 minute â€” your app URL will appear (e.g. `https://yourusername.github.io/street-medicine-app/`)

### Step 4 â€” Add to iPhone Home Screen

1. Open the URL in **Safari** on your iPhone
2. Tap the **Share** button (box with arrow)
3. Scroll down â†’ tap **"Add to Home Screen"**
4. Tap **Add**

The app now appears as a full-screen app on your home screen with the medical cross icon.

---

## Features

| Feature | Details |
|---|---|
| **Rounds** | Create a round per shift (date, area, volunteers) |
| **Encounters** | Full structured form per patient (demographics, vitals, exam, assessment, interventions, follow-up) |
| **Non-medical contacts** | Quick logging of supplies-only contacts |
| **Round summary** | Auto-counts + free-text summary |
| **Photos** | Camera + library, auto-resized for storage |
| **Export** | iOS Share Sheet (â†’ Apple Notes) + PDF download |
| **Offline** | Works with no internet after first load |
| **Storage** | All data stored locally on device only |

---

## Data & Privacy

All data is stored in `localStorage` on your device. Nothing is sent to any server.
To back up your data, use the Export function regularly.

---

## Export Format

The Share Sheet exports a plain-text report matching your existing Apple Notes template format, including:
- Round header (date, location, volunteers)
- Each encounter (address, demographics, vitals, exam, assessment, interventions, follow-up)
- Non-medical contacts table
- Round summary

The PDF export mirrors the same format with photos appended at the end.
