# Screenshots

Eight images, 1080 x 1920, English. They replace the earlier twelve-image set.

## How they are built

They come from the app's own design material, not from a stock mockup builder:

- **Palette** — taken from `ui/theme/Color.kt` (the same indigo/cyan/amber and category accents the app uses).
- **Icons** — the same 24 line icons the app draws in its lists and tool tiles.
- **Type** — Space Grotesk for headings, Outfit for body text, at the same relative sizes as the app.
- **Layout** — 410 x 820 dp phone body, 16 dp margins, the same card radii and row heights as the app.

Each image pairs a headline with four feature cards and one screen: tags and MultiTagPlay, folder play
with its nine orders, the file manager home, the download queue, the browser, the ZIP reader, the photo
editor and the encrypted folder container.

## Accuracy rules used for captions

- "Nine orders" — the app has exactly nine playback orders.
- No ad-block counter is claimed anywhere: the live counter belongs to the data saver.
- The vault is described as `.enx` with an AES-256-GCM key derived by PBKDF2, plus the folder container.
- Sizes and counts on the screens (128 GB of 256 GB, 231 music files, 18 blocked items) are illustrative
  of the UI layout, not measurements of a specific device.

## Files

| File | Screen |
|---|---|
| `01-files-and-tags.jpg` | Tag list, selection bar, recently tagged |
| `02-folder-play.jpg` | Folder play sheet with kinds, orders, continue |
| `03-files-home.jpg` | Storage card, categories, recent files, tools |
| `04-downloads.jpg` | Queue, scheduled item, duplicate check, destination |
| `05-browser.jpg` | Tab groups, data saver, privacy, closed tabs, stats |
| `06-zip.jpg` | Archive browsing, extract, play prompt, paste |
| `07-editor.jpg` | Crop, tone curve, exposure, draft, export |
| `08-encrypted-folder.jpg` | Locked container, `.enx` entries, vault |
