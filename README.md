# 🏥 Street Medicine App

A mobile-first progressive web app (PWA) for documenting street medicine rounds. Built as a single HTML file — no server, no database, no installation required.

## Features

- **Medical encounters** — chief complaint, vitals, exam, assessment, interventions (wound care, medication, supplies, referrals), follow-up notes
- **Non-medical contacts** — location, name/alias, supplies given
- **Photos** — attach photos to encounters and referrals
- **Maps** — encounter locations plotted on a map per round and across all rounds
- **Address autocomplete** — Tel Aviv street names with live suggestions
- **Stats** — supplies summary and map filtered by month or all-time
- **Export** — copy rich report (with inline photos) to Apple Notes, or download as PDF
- **Offline** — all data stored locally on the device, works without internet after first load

## Installing on iPhone

1. Open the app URL in **Safari**
2. Tap the **Share** button (box with arrow)
3. Tap **"Add to Home Screen"**
4. The app appears as an icon on your home screen and launches full-screen

> First open requires an internet connection to load map and PDF libraries. After that, core functionality works offline.

## Updating

The app is a single file. When a new version is uploaded to GitHub, everyone gets the update automatically the next time they open the app with an internet connection — no re-installing needed.

## Data & Privacy

All data is stored **locally on your device** using the browser's localStorage. Nothing is sent to any server. Clearing your browser data or deleting the app will erase all records — export important rounds before doing so.

## Tech

- Vanilla HTML / CSS / JavaScript — no framework, no build step
- [Leaflet.js](https://leafletjs.com/) for maps
- [CartoDB Positron](https://carto.com/basemaps/) tiles
- [Nominatim](https://nominatim.org/) (OpenStreetMap) for geocoding
- [jsPDF](https://github.com/parallax/jsPDF) + [html2canvas](https://html2canvas.hertzen.com/) for PDF export
