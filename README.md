# Exployer — official Android releases

Signed release builds of **Exployer**, the all-in-one Android file manager, video downloader,
browser and photo editor by [Baloch Script](https://balochscript.com).

**Download the latest APK:** [balochscript.com/exployer-android-file-manager-video-downloader](https://balochscript.com/exployer-android-file-manager-video-downloader/)

## Latest

| Version | Android | Package |
|---|---|---|
| 0.9.37 (versionCode 47) | 8.0+ | `com.balochscript.exployer` |

Every release here is signed with the same key as the version on the website, so updating over
an older install works without uninstalling.

## Verify what you downloaded

1. Download the APK from the **Releases** panel of this repository only.
2. Compare its SHA-256 with the value published on the release page and in the post:

```
# Windows
certutil -hashfile exployer-0.9.37.apk SHA256
# Linux / macOS
shasum -a 256 exployer-0.9.37.apk
```

A file from anywhere else is not ours, even if the name matches.

## Install

1. Copy the APK to the phone and tap it.
2. If Android asks, allow installing from this source for your browser or file manager.
3. Grant the "All files access" permission on first launch — it is what the file manager needs.

There is no account, no sign-in and no upload: files, history and the vault stay on the device.

## Links

- Website and feature guide: https://balochscript.com
- Source code: private repository (not published)
- Support: balochscript@gmail.com
