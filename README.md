# Through the Ages Tracker

Tracks culture, science and military for *Through the Ages* on a phone or tablet lying in the middle of the table.

## Files

| File | What it does |
|---|---|
| `index.html` | The whole app |
| `manifest.webmanifest` | Name, icons and colours; tells Android to open the app without browser bars |
| `sw.js` | Saves the app on the device so it also works offline |
| `icons/` | App icons, including the round-cropped variant Android uses |

## Publish on GitHub Pages

1. Create a repository, for example `tta-tracker` (public on a free account).
2. Upload all files, keeping the `icons` folder.
3. Settings → Pages → Build and deployment → Deploy from a branch → `main`, `/ (root)` → Save.
4. After a minute or two the app is at `https://<username>.github.io/tta-tracker/`.

## Install on Android

1. Open the address above in Chrome.
2. Menu (⋮) → **Install app** (on some phones: **Add to Home screen** → Install).
3. Start it from the new icon. It opens without the address bar and works without a connection.

Games are stored on the device. The installed app and Chrome share the same saved game.

## Updating

Upload a new `index.html` over the old one. The app picks it up the next time it is opened with a connection.

The app is locked to portrait orientation, so it doesn't flip when the phone lies flat on the table. For a tablet in landscape, change `"orientation": "portrait"` to `"landscape"` in `manifest.webmanifest`, or to `"any"` to follow the device.
