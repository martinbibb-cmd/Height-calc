# Height-calc

A lightweight standalone **Building Height Check** app for estimating building height from:

- manual distance input (distance to wall base)
- captured base angle
- captured top angle

Core formula:

`H = d * (tan(theta_top) - tan(theta_base))`

## Run

Open `index.html` in a browser.

## Workflow

1. Enter distance to building (metres, m)
2. Choose angle entry mode:
   - **Manual entry**: type base and target/top angles directly
   - **Automatic camera**: open a fullscreen camera view, aim using overlay crosshairs + green horizon line (which stays level and moves up/down with pitch), then store base and target
3. Press **Calculate** to close camera view and show height from base in metres
4. Use **Reset** to start from scratch
5. Use **?** to show/hide the full maths breakdown for the current result

Includes validation for missing or invalid values.

## PWA install

The app now includes:

- `manifest.webmanifest`
- `sw.js` service worker
- app icons (`icon-192.png`, `icon-512.png`)

When served over HTTPS (or localhost), it can be installed as a PWA.
