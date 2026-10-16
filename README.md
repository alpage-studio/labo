# Labo Darkroom

One look for the whole roll, a correction for every photo.

- **Import** a whole roll at once (JPEG, PNG, WebP, or RAW through its embedded preview).
- **Pick a look** on the negative strip: each look is previewed on your own photo.
- **Save**: on a phone, one share sheet sends every photo to the gallery; on a computer, a ZIP or separate files.

Everything runs on the device. No photo is uploaded. Works offline once installed.

## Files

| File | Role |
|---|---|
| `index.html` | the whole app (HTML, CSS, JS) |
| `manifest.webmanifest` | name, icons, full-screen mode for installing |
| `sw.js` | offline support; **bump `VERSION` on every release** |
| `jszip.min.js` | JSZip 3.10.1 (MIT), for the ZIP export |
| `icon-*.png`, `apple-touch-icon.png` | icons |

## Install on a phone

- **iPhone (Safari)**: open the address → Share → **Add to Home Screen**.
- **Android (Chrome)**: open the address → ⋮ menu → **Install app**.

## Release

Edit the files, bump `VERSION` in `sw.js`, commit, push to `main`. GitHub Pages serves the new version; the app picks it up the next time it opens online.
