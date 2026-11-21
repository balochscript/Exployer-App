# Changelog

All released builds are published in [Releases](../../releases). The APK is signed with the same key
for every version, so updates install over the previous build without wiping data.

Builds between 0.9.91 and 0.9.102 were internal only; everything they contained is described in the
0.9.103 entry below, because 0.9.103 is the first public build since 0.9.90.

---

## 0.9.103 — versionCode 113

Two files, same features: `exployer-0.9.103.apk` (9.1 MB, optimised with R8) and
`exployer-0.9.103-nor8.apk` (18.0 MB, same code without minification).

### New features

- **MultiTagPlay** — long-press several tags in the tag list, then play everything they contain as one
  queue. A file shared by two selected tags is played once, not twice. The selection bar offers
  "select all" (honouring the current tag search), the order menu keeps all nine orders, and the queue
  remembers its own filters separately from single-tag playback.
- **Quick tagging while you browse** — long-press a file in the list, select it and tap the tag button
  in the selection bar; the same tag action also lives in the video/photo viewer and on Now Playing.
  There is no cap on how many tags a single file can carry.
- **New encryption format `.enx` (AES-256-GCM, chunked) with an encrypted folder container** — a folder
  encrypted with Exployer can now be opened and browsed like any other folder, file by file, after one
  password prompt. Files are sealed in chunks, so a very large file no longer has to be read into memory
  in one piece. Files encrypted by older versions (`.enc`) are still readable; rename them to `.enx` and
  the app picks them up. The app shows that hint itself.
- **Editor export runs in the background** — close the editor, leave the app, or switch to another app:
  the photo or video is still produced, with a progress notification (and cancel, done, failed,
  cancelled and system-timeout states). Video export now survives the system's background time limit.
- **Six new interface languages** — Spanish, Brazilian Portuguese, Indonesian, Hindi, Arabic and Urdu,
  alongside Persian and English, plus "system language".
- **Full Persian and right-to-left review** — letter spacing removed everywhere (it was breaking Persian
  letter joining), line heights corrected for Persian, notification text now follows the app language
  instead of the system language, and the whole UI was re-checked in RTL.
- **Media sniffer is per page, not per tab** — opening another page clears the previous page's stream
  list instead of mixing old and new videos; a same-domain navigation no longer keeps stale entries.
- **Clear rewarded-ad rule** — one completed rewarded video turns ads off for 24 hours; five videos
  within those 24 hours give a full week. The counter starts with the first video and warns before reset.
- **Restore of the previous playback** — every folder, archive, tag and multi-tag selection keeps its own
  saved queue, so "continue at 7 of 42 · least played" is offered the next time you open the same place.
- **Recently closed tabs** — kept for 24 hours, restorable in one tap.
- Browser: browser statistics screen (total and weekly visits, downloads, top sites), per-site zoom that
  can be remembered per site, HTTPS/HTTP indicator in the address bar, tab previews, eight group colours.
- Downloads: scheduled downloads with retry count, delay, stop policy and deadline; duplicate detection
  ("already downloaded", "already in queue"); checksum verification; separate All / Active / Scheduled
  tabs with progress, speed and status sorting.

### Fixed

- Silent crash on launch (an application context used before it existed) — fixed.
- Endless app-chooser loop when installing an APK from the file list — fixed.
- Play counts were wrong: every tap on Next counted as a play, so "least played" and "most played" were
  effectively the scan order. A play now counts only after 10 seconds or 25 % progress.
- Tag play button ignored the chosen order and always started alphabetically — fixed.
- Tab bar jumped and the address bar selected a single word — both fixed.
- Background session writing was missing saves and rewriting the session file hundreds of times per
  minute; both fixed, so restore is reliable.
- Video export could be killed by Android's background limit without a word — now reported and resumable.
- Status-bar icons now follow the app theme instead of staying light on a dark theme.

### Under the hood

- The release build is shrunk and optimised with R8: **18.0 MB → 9.1 MB** for the same feature set.
- The unshrunk build is still published so an unusual device can fall back to it.

---

## 0.9.90 — versionCode 98

- Rewarded ads reworked: one video turns ads off for 24 hours, five videos within that window give a
  full week, with a visible counter and reset warning
- Download queue: pause all / resume all, notification permission prompt, battery-optimisation hint
- Video editor: normalise merged clips by matching the first clip or the largest one
- Photo editor: heal brush stroke control, perspective correction, three save targets
- Browser: data saver with a live blocked-items counter and "load all"

## 0.9.37 — versionCode 47

- Fullscreen video: the system bars hide away, manual rotation and a one-tap screenshot
- Select from the first file to the last in one action
- ZIP: extract a single folder or file, add files to an archive, Zip-Slip protection
- File tagging and playback of everything that shares a tag
- Download errors now state the real reason: DRM, 403/404, an HTML page, network, low storage
- Browser menu regrouped: page, text size, tools, modes, settings
- Folder playback includes subfolders; one unified queue (music to video)
- Three-state repeat and shuffle in the player
- Fixed the rewarded-ad counter, plus ZIP reader, breadcrumb and copy bugs

## 0.9.36 and earlier

Release notes for each older build are on the [Releases](../../releases) page; each one lists its own
changes. Downloads for previous versions stay available there.

| Version | APK size (as published) |
|---|---|
| 0.9.103 (R8) | 9.1 MB |
| 0.9.103 (no R8) | 18.0 MB |
| 0.9.90 | 8.6 MB |
| 0.9.37 | 16.6 MB |
| 0.9.36 | 16.6 MB |
| 0.9.30 | 16.5 MB |
| 0.9.25 | 16.4 MB |
