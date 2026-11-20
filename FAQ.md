# Exployer — frequently asked questions

### Is Exployer really free?

Yes. There is no account, no subscription and no paid tier. The app is supported by ads, and rewarded
videos turn them off: **one completed video gives 24 hours without ads, and five videos inside those
24 hours give a full week**. The counter starts with your first video, shows how many videos are left,
and warns you before it resets.

### Which file should I download — the 9.1 MB one or the 18.0 MB one?

Start with `exployer-0.9.103.apk` (9.1 MB). It is the same app, shrunk and optimised with R8. The
`-nor8` build is the identical code without minification and exists only as a fallback for a device
where the small build misbehaves. Both are signed with the same key, both are versionCode 113, and they
can update each other.

### Does it need root?

No. It uses Android's **All files access** permission, which you grant once on first launch.

### Which Android versions are supported?

Android 8.0 (API 26) and newer, including Android 13–16 with the newer media permissions. The app
targets API 36.

### Does it work offline?

The file manager, both players, the photo and video editor, the ZIP reader and the vault work with no
connection at all. Only the browser and the video downloader need a network.

### Can I download videos from Instagram, YouTube or TikTok?

Exployer saves streams that a page loads as plain media — MP4, HLS (M3U8) or DASH — which covers a
large part of the web. It cannot save DRM-protected streams and does not bypass paywalls or logins,
and it tells you so instead of writing a broken file. Always respect the site's terms and the rights
of the creator.

### Why do I get "DRM protected" on some sites?

Because those services encrypt the stream by design. No downloader can produce a playable file from
it; Exployer reports the real reason instead of failing silently.

### Where are my downloads saved?

By default to `Downloads/Exployer`, split into subfolders for video, audio, images and files. You can
change the destination folder in the download settings.

### Can I recover a file I deleted?

Yes, if you deleted it inside Exployer: it goes to the recycle bin and stays recoverable for up to
30 days. Files deleted by other apps never reach that bin.

### What are tags, and how do I use them?

Tags are your own labels for files and folders. Add one from the file list, from the Now Playing
screen, or while viewing a photo or video, so you never have to leave what you are doing. You can tag
several files at once, give a tag one of ten colours, sort tags five ways, and play everything under a
single tag. Long-press several tags to play them together — this is called MultiTagPlay, and a file
that belongs to two selected tags is played only once.

### What happens to my encrypted files from older versions?

Files ending in `.enc` are still readable. Rename them to `.enx` (for example `report.pdf.enc` →
`report.pdf.enx`) and the app will recognise them. New files are always sealed in the `.enx` format:
AES-256-GCM in chunks with a PBKDF2-derived key. A folder you encrypted can be opened like a normal
folder — one password prompt, then you browse it.

### Can Exployer open a password-protected ZIP?

No. Standard ZIP archives are fully supported — browsing, extracting, adding files and playing media
inside the archive — but encrypted ZIPs are not.

### Does it have a dark theme?

Yes. Follow the system theme, or force light or dark, and pick one of five accent palettes.

### Does the app work right-to-left?

Yes — it is built RTL-first. Eight interface languages are bundled (Persian, English, Spanish, Brazilian
Portuguese, Indonesian, Hindi, Arabic, Urdu) and the interface language can be changed in Settings,
independently of the phone's language. Notifications follow the same choice.

### How do I remove the ads?

Watch rewarded videos in the ads section: one video gives 24 hours without ads, five videos inside
those 24 hours give a full week.

### Are my files uploaded anywhere?

No. Files, playback history, tags, recycle-bin entries and the vault stay on the device. Camera,
microphone and location are only exposed to a site you opened, only after you approve it for that site.

### Is it safe to install the APK from here?

Check the SHA-256 published in the [README](README.md#verify) and on the release page, and install only
from this repository or [balochscript.com](https://balochscript.com). Every release is signed with the
same key, so a tampered file would be rejected by Android on update.

### Is Exployer on Google Play or Cafe Bazaar?

It is published on Cafe Bazaar (`com.balochscript.exployer`); that listing can lag a few versions
behind. This repository always hosts the newest signed APK first.
