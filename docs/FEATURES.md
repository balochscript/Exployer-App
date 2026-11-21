# Exployer — every feature, in detail

Version 0.9.103 (versionCode 113) · Android 8.0+ · no root · no account

This document describes what the app actually does, including the small behaviours that are usually
left out of store pages. If a feature is not here, it is not in the app.

---

## 1. File manager

- **Storage**: internal storage and SD card side by side.
- **Views**: list and grid.
- **Sort**: name, date, size or type, each in both directions; in the tag and archive lists, folders stay
  above files and only the files are shuffled by "random".
- **Navigation**: a tappable breadcrumb jumps to any parent folder in one tap.
- **Search**: global search across the whole storage, with the same actions as a folder list.
- **Selection**: single, multi-select, and "first to last" range select.
- **Actions**: copy, move, delete, rename, share, properties.
- **Copy/move sheet**: its own breadcrumb, so you can create a folder and paste without leaving the sheet;
  hidden files can be shown there too.
- **Categories**: audio, video, images, documents, downloads, APKs, archives — plus a live storage card
  (used / free / total) on the home screen.
- **Recent files**: everything changed in the last five days, with a type filter, open-containing-folder,
  properties, and an honest note when the storage was too large to be scanned completely.
- **Documents**: a built-in PDF viewer and a built-in text viewer, so a document does not need another app.
- **APKs**: install an APK straight from the list (the "install unknown apps" permission is optional and
  only used for this).
- **Compress**: create a ZIP from a selection.

## 2. Tags

- **Instant tagging** from three places: the file list, the Now Playing screen, and the photo/video viewer.
  You never have to leave what you are doing to label a file.
- **Bulk tagging**: select many files and apply a tag in one action. The picker shows "3 of 5" when only
  part of the selection already carries that tag.
- **Ten colours**, assigned automatically to new tags.
- **Tag management**: create (including from inside the picker), rename, delete. Deleting a tag never
  deletes files — the dialog says so.
- **Validation**: a tag cannot be empty and a duplicate name is rejected.
- **Search**: search inside the tag list.
- **Five sort orders** for tags: most items, fewest items, newest, oldest, recently tagged.
- **Tag playback**: play only the music in a tag, or all of its media, using the same nine orders and the
  same kind filter as folder play, with its own saved session.
- **MultiTagPlay**: long-press tags to enter selection mode, then select several. The bar offers close,
  "N tags selected", "select all" (honouring the current search) and play. The play menu offers "continue
  previous playback" (only for the exact same set of tags), music-only or all-media with counts, kind
  chips with counts, and the order menu with all nine orders. A file that belongs to two selected tags
  is queued once.

## 3. Smart folder play

- **Scope choice**: "play this folder's music, with subfolders (N)" or "play all media in this folder,
  with subfolders (N)" — both with live counts.
- **Recursive**: the whole tree, not just the first level, up to 24 levels deep and 20,000 files. If the
  limit is actually hit, the app says "only the first 20,000 files are included" instead of pretending.
- **Honest skips**: folders that could not be opened (no permission) and folders deeper than the limit
  are counted and reported.
- **Nine orders**: name A→Z, name Z→A, date newest, date oldest, size largest, size smallest,
  least played, most played, fully random.
- **Kind filter**: music / video / images chips with counts, switchable before you press play. If the file
  you tapped is excluded by the current chips, the filter is ignored for that tap — you chose that file
  on purpose.
- **Continue previous playback**: each folder, archive, tag and multi-tag set keeps its own session
  (queue, order, kind filter and current item) on disk. The menu then offers
  "continue at 7 of 42 · least played".
- **What counts as a play**: only after 10 seconds of real playback or 25 % progress. Without this,
  pressing Next thirty times would mark thirty files as played and "least played" would just mirror the
  scan order.
- **Queue rules**: adding to the queue extends the session queue too, so next/previous follow what you
  added; duplicates are allowed but never silently dropped by shuffle; removing an item removes one
  instance, not every copy.
- **One queue**: if the next item is a video, the video player opens with the same queue.

## 4. Music player

- Library with silent refresh (new tracks are picked up without a full rescan).
- Queue, add to queue, reorder, remove.
- Playback speed, sleep timer with remaining time, repeat off / all / one, shuffle.
- Equalizer with presets, bass boost and a virtualizer, with a reset.
- Always-visible mini player.
- Background playback with notification controls.

## 5. Video player

- Horizontal drag to seek, vertical drag for volume and brightness.
- Adjustable swipe-seek range, 0.5 % to 20 %, so a small movement never jumps a scene.
- Double tap to pause/play, hold for 2× speed.
- Touch lock (with a visible unlock hint).
- Aspect ratio: fit, crop to fill, stretch.
- Audio track and subtitle track selection where the file provides them.
- Fullscreen without system bars, manual rotation.
- Picture-in-picture.
- One-tap screenshot.
- End-of-video behaviour: replay, stop, or next video.
- Companion media: attach an image or another video that opens alongside.
- Crop and trim straight from the player.

## 6. Browser (Baloch Core)

Rendering is done by the system Chromium WebView; everything around it — tabs, blocking, privacy, stats,
downloads — is Exployer's own code, and the user agent identifies itself as Baloch Core.

- **Tabs**: multiple tabs, tab previews, new tab, close, switch.
- **Tab groups**: create, rename, colour (eight colours), move a tab into a group by dragging its card
  onto the group chip or onto "Ungrouped"/"All tabs", close a whole group (with a warning that the tabs
  stay restorable for 24 hours).
- **Incognito tabs**: separate policy, nothing is kept.
- **Recently closed tabs**: kept for 24 hours, restore in one tap.
- **Session restore**: tabs, their pages and the exact scroll position are saved and reopened. Tabs are
  never closed automatically.
- **Tab bar placement**: top, bottom, left (vertical), right (vertical), hidden.
- **Tab appearance**: full title or favicon only.
- **Bottom action bar**: optional.
- **Ad blocking**: a curated list of common advertising domains is blocked at the request level, plus CSS
  that hides common ad slots. It is a first line of defence, not a full subscription-based blocking engine.
- **Data saver**: heavy images and media on a page are held back until you tap "Load all", and the toolbar
  shows how many items were blocked on the current page.
- **Privacy**: an optional Do Not Track / Sec-GPC switch (off by default) that sends both headers on
  every request when enabled; clear history, cache and cookies on exit.
- **Home page**: either the built-in Baloch Core page or a blank page; shortcuts can be edited; a custom
  search-engine template can be entered (`%s` is replaced by the query).
- **Find in page**: next and previous match.
- **Text and zoom**: default text size, zoom in/out, and a zoom level that can be remembered per site.
- **Desktop mode**: request the desktop version of a site.
- **Address bar**: HTTPS/HTTP indicator, select and copy the address.
- **Context menu on links**: open in new tab, open in incognito tab, copy link; on images: save image.
- **Bookmarks** and **history**, with clear.
- **Statistics**: total visits, total downloads, weekly visits and downloads, last 7 days, most visited sites.
- **Site permissions**: camera, microphone and location are requested per site; you can ask, allow or deny,
  "remember for this site", and manage the saved decisions later (removing one means you will be asked again).
- **Passwords**: autofill with the phone's password manager.

## 7. Download manager

- **Media sniffer**: an icon in the address bar or a draggable floating bubble (its position is remembered)
  lists every video and audio stream on the current page with its exact size. The list belongs to the page,
  not the tab, so navigating to another page clears it instead of mixing old streams in.
- **Before downloading**: rename the file, copy the direct link, choose the quality (auto/source), rescan.
- **Queue**: percentage, speed, size, ETA, and the position in the queue.
- **Parallelism**: 1 to 15 files at once, or unlimited. Extra files wait in the order you added them and
  start as soon as a slot frees up.
- **Resume**: continues from the exact byte; a partially downloaded file is kept and the UI says so.
- **Retries**: 3 to 30 automatic retries, or unlimited, with an optional custom delay between attempts;
  a stop policy decides whether the engine keeps trying, stops on the first error, or stops at a deadline.
- **Scheduled downloads**: pick a date and time, a retry count, a delay, a stop policy and a deadline.
  Schedules live in a file, survive app kills and are re-armed after a reboot.
- **Duplicates**: "already downloaded" and "already in the download queue" are detected; a failed previous
  attempt is reported as safe to retry.
- **Integrity**: when the server announces a checksum, the finished file is verified and discarded on a
  mismatch (one automatic retry).
- **Errors, honestly named**: DRM-protected, 403/404, an HTML page returned instead of a file (anti-leech),
  network failure, storage full or no permission, conversion/recording failure, deadline reached — each with
  the next step you can take and an expandable technical detail.
- **Streams**: HLS (M3U8) and DASH, with a capture fallback when no single file exists.
- **Destination**: `Downloads/Exployer` by default, or any folder you pick.
- **Controls**: pause or resume everything at once (new and scheduled downloads wait too), per-item pause/
  start/retry/open/share/delete, batch selection and batch delete, clear the finished list (files stay).
- **Sorting**: by progress, speed or status; separate All / Active / Scheduled tabs.
- **Notifications**: a dedicated channel with progress, paused, completed and failed states; if notification
  permission is off the app says so and offers to enable it.
- **Background**: a hint to set Exployer to "Unrestricted" in the battery settings, and an explicit message
  when Android's background transfer limit pauses a download.

## 8. Photo editor

- Free crop with output pixel size shown, rotate.
- Eight light and colour sliders: exposure, contrast, highlights, shadows, saturation, vibrance,
  temperature, tint.
- Tone curve with free control points, plus ready-made curves.
- Six filters (warm, cool, vivid, faded, mono, film) that are a starting point, not a locked look.
- Heal brush with adjustable size, last-stroke undo and clear-strokes.
- Perspective correction by dragging four corners onto the document or wall corners.
- Undo and redo with confirmation.
- Automatic draft, so leaving the editor does not lose the work.
- Three save targets: beside the original, `Download/Exployer/Edit`, or replace the original (the previous
  copy goes to the recycle bin).

## 9. Video editor

- Trim, crop, rotate.
- Merge several clips with automatic dimension normalisation — match the first clip or match the largest.
- Add clips from the internal file picker or the system picker.
- Export in the background with a progress notification: cancel, done (tap to open), failed, cancelled and
  system-timeout states are all surfaced; a background export interrupted by Android's time limit can be
  retried without losing the source part.

## 10. ZIP reader

- Browse an archive like a folder: breadcrumb, up, open subfolders — nothing is extracted to look around.
- Extract the folder you are currently in, or a single file or folder, next to the archive, with byte-based
  progress and a specific message when there is not enough space.
- Paste files into an archive (the archive is repacked in place).
- Zip-Slip protection.
- A central-directory index and cache, so very large archives open quickly and keep their listing.
- Play the media inside an archive, subfolders included, with the same nine orders and kind filter. Because
  playback needs real files, the app asks first — "12 files must be extracted to temporary storage" — and
  then plays with the same queue behaviour as the file manager.
- Open a non-media entry (document, text, APK) with the built-in viewer or an external app.

## 11. Encryption and the password vault

- **`.enx` format**: chunked AES-256-GCM with a PBKDF2-derived key. Chunking means a huge file is sealed
  without being held in memory in one piece.
- **Encrypted folder container**: a folder encrypted by Exployer opens like a normal folder after one
  password prompt; you can browse and read inside it. Locking hides it again.
- **Options**: delete the originals after encryption (with an explicit warning that this is permanent and
  not a recycle-bin move), or keep them.
- **Compatibility**: files from older versions (`.enc`) are still readable; rename them to `.enx`.
- **Limits reported, not hidden**: "this item is not an Exployer encrypted file", "the file is damaged or
  incomplete", "this folder has too many items to encrypt (limit 20,000)".
- **Password vault**: a master password you set once, entries with site, username, password and an optional
  note, instant lock, master-password change, and deletion with confirmation. The master password is never
  stored; without it, the entries cannot be read.

## 12. Storage tools

- **Recycle bin**: deleted files stay recoverable for 30 days, with a countdown, restore and permanent delete.
- **Storage analysis**: total used, biggest folders, biggest files, split by kind — including torrent files.
  When the scan had to stop early it says so.
- **Duplicate finder**: groups of identical files, "remove extra copies" moves the extras to the recycle bin.

## 13. Look, language and settings

- Theme: system, light, dark.
- Five accent palettes.
- Eight languages: Persian, English, Spanish, Brazilian Portuguese, Indonesian, Hindi, Arabic, Urdu —
  independent of the phone's language; the app even applies it to notifications.
- Playback settings: swipe-seek range, video end behaviour, mini player, background playback.
- File settings: show hidden files.
- Browser settings: appearance, tab bar placement, home page, shortcuts, search engine and template,
  text size, ad blocking, data saver, password autofill, clear on exit, restore tabs, Do Not Track,
  site permissions, downloads, media detector and its button placement.
- Download settings: destination, parallelism, auto-start, retries, retry delay, stop policy,
  notifications, battery.

## 14. Ads

The app is free and supported by advertising (Tapsell). Rewarded videos remove ads:

- One completed rewarded video → 24 hours without ads.
- Five completed videos within those 24 hours → a full week without ads.
- The counter starts with the first video, shows progress, and warns before it resets. A reward is only
  recorded after the video is confirmed as watched.

## 15. What Exployer does not do

- No DRM circumvention, no login or paywall bypass: DRM-protected streams are reported as such.
- No password-protected ZIP archives.
- No cloud, no sync, no account, no cross-device backup.
- No analytics or crash-reporting SDK; nothing about your files leaves the phone.
- Ad blocking is a curated domain list plus ad-slot hiding, not a subscription-list engine.
