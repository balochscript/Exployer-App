# Exployer — frequently asked questions

### Is Exployer really free?

Yes. There is no account, no subscription and no paid tier. The app is supported by ads; watching
five rewarded videos gives you seven days without ads. The counter uses a 24-hour window and warns
you before it resets.

### Does it need root?

No. It uses Android's **All files access** permission, which you grant once on first launch.

### Which Android versions are supported?

Android 8.0 (API 26) and newer, including Android 13–16 with the newer media permissions.

### Does it work offline?

The file manager, both players, the photo and video editor, the ZIP reader and the vault work with no
connection at all. Only the browser, the ad-blocker filter updates and the video downloader need a
network.

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
change the destination folder in Settings.

### Can I recover a file I deleted?

Yes, if you deleted it inside Exployer: it goes to the recycle bin and stays recoverable for up to
30 days. Files deleted by other apps never reach that bin.

### Does it have a dark theme?

Yes. Follow the system theme, or force light or dark, and pick one of five accent colours.

### Does the app work right-to-left?

Yes — it is built RTL-first. Every bundled translation is complete and the interface language can be
changed in Settings.

### How do I remove the ads?

Watch five rewarded videos in the ads section: you get seven days without ads.

### Are my files uploaded anywhere?

No. Files, playback history, tags, recycle-bin entries and the vault stay on the device. Camera,
microphone and location are only exposed to a site you opened, only after you approve it.

### Is it safe to install the APK from here?

Check the SHA-256 published in the [README](README.md#verify) and on the release page, and install only
from this repository or [balochscript.com](https://balochscript.com). Every release is signed with the
same key, so a tampered file would be rejected by Android on update.

### Is Exployer on Google Play or Cafe Bazaar?

A Cafe Bazaar release is in progress. This repository always hosts the newest signed APK first.
