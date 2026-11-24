# RACEFACE Designer 🏁

A mobile-first progressive web app for building racing-inspired watch-face artwork, with a 466 × 466 export canvas intended for the CMF Watch Pro 2 custom-background workflow.

## What it does

- Live circular watch preview
- Racing Red/Yellow, Monochrome, Ice Blue and Neon presets
- Editable accent and secondary colors, brand text and race number
- Toggle circuit graphic, race car, checkered strip and carbon-fibre texture
- Export a 466 × 466 PNG
- Installable PWA with offline caching
- Works in desktop and mobile browsers

## Compatibility note

RACEFACE is a **watch-face artwork designer**, not firmware and not a companion app. It cannot replace the CMF Watch Pro 2 operating-system interface, install arbitrary watch apps, or transfer a face over Bluetooth. Exported images are intended to be tried through the official CMF companion app's supported custom-face/background workflow. Exact import support and which fields can be overlaid are determined by the watch and companion-app versions. The visual preview contains sample values; it does not read live watch sensors.

## Run locally

Open `index.html` in a browser. For PWA installation and service-worker/offline features, use HTTPS or localhost.

## Deploy on GitHub Pages

1. Create a public repository named `raceface-designer`.
2. Upload the contents of this folder to the repository root (not the enclosing folder).
3. In **Settings → Pages**, choose **Deploy from a branch**.
4. Select branch `main` and folder `/ (root)`, then save.
5. Open the Pages URL on Android Chrome and choose **Install app** or **Add to Home screen**.

## Termux

After creating the repository, replace `YOUR-USERNAME` with your GitHub username:

```bash
pkg update -y
pkg install git python -y
git clone https://github.com/YOUR-USERNAME/raceface-designer.git
cd raceface-designer
python -m http.server 8080
```

Open `http://127.0.0.1:8080` on the same phone. For PWA installation, use the HTTPS GitHub Pages URL.

## Project files

- `index.html` — complete designer UI and PNG export logic
- `manifest.json` — PWA manifest
- `sw.js` — service worker and offline cache
- `icon.svg` — app icon
- `LICENSE` — MIT license

## License

MIT. See `LICENSE`.
