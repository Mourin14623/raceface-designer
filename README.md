# RACEFACE Studio 🏁 v2.0

A mobile-first racing-inspired watch artwork studio. Design, preview, save, and export a circular 466 × 466 watch-face graphic.

## 2.0 upgrades
- Redesigned Studio cockpit UI for phone and desktop
- 8 palettes: Race, Mono, Ice, Neon, Apex/Sunset, Green, Silver, Pink
- Live clock/date with 12/24-hour formats
- 3 face layouts: Race cockpit, Minimal, Grid/Telemetry
- Customize colors, brand/team text, race number
- Toggle carbon, circuit graphic, race car, checkered strip, outer ring, minute ticks, stats and weather card
- Local Garage: save/load/delete designs (up to 30)
- Randomize colors and race number
- Export 466×466 PNG and SVG
- PWA installation and offline caching

## Use
Choose Style, Layout and Details, then save in Garage or export PNG/SVG. Garage saves stay on the current device/browser.

## GitHub Pages
Repository Settings → Pages → Deploy from a branch → main → /(root) → Save.

## Termux
```bash
pkg update -y
pkg install git python -y
git clone https://github.com/Mourin14623/raceface-designer.git
cd raceface-designer
python -m http.server 8080
```
Open http://127.0.0.1:8080.

## Compatibility
Artwork designer only—not watch firmware or a companion app. It cannot modify the watch OS, Bluetooth-transfer faces, or read live sensors. Weather, steps and pulse are decorative sample values. Applying artwork depends on supported customization features in the watch and companion app.

## Files
- index.html — app
- manifest.json — PWA config
- sw.js — offline cache
- icon.svg — app icon
- LICENSE — MIT
