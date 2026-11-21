# Privacy — Exployer

**Short version: your files never leave your phone. There is no account and no sign-in.**

## What stays on the device

- Files and folders you open, move, rename, compress, encrypt or delete
- Playback history and play counts, queues, saved playback sessions, tags, and the recycle bin
- The password vault and every `.enx` encrypted file or encrypted folder (AES-256-GCM with
  PBKDF2-derived keys) — the master password is never stored anywhere and cannot be recovered by us
- Browser history, bookmarks, saved logins, statistics and site permissions, unless you enable clear-on-exit

None of this is uploaded, synced or backed up by Exployer.

## Permissions and what they are for

| Permission | Why |
|---|---|
| All files access | Managing files and folders is the core of the app |
| Camera, microphone, location | Only handed to a site you opened, and only after you allow it for that site. You can deny, allow, or remember the choice per site |
| Notifications | Playback controls, download progress and editor-export progress |
| Install unknown apps (optional) | Only if you choose to install an APK from inside the file manager |
| Battery optimisation exemption (optional) | Only so long downloads and background exports are not stopped by the system |

## Ads

Exployer is free and supported by advertising delivered by a third-party ad network (Tapsell). That
network may collect device and advertising identifiers as described in its own privacy policy; it does
not receive your files, your history or the contents of your vault. Rewarded videos remove ads: one
video for 24 hours, five videos within those 24 hours for a full week.

## Network use

The browser and the downloader are the only parts that talk to the internet, and only with addresses you
open or request. The app contains no analytics or crash-reporting SDK of its own. There is no self-update
mechanism and no background phone-home.

## Encrypted data

Files encrypted with `.enx` are sealed with a key derived from your password (PBKDF2) and AES-256-GCM in
chunks. If you lose the password, the data cannot be recovered — by us or by anyone else. The unencrypted
originals are only kept if you explicitly choose to keep them.

## Children

The app is not directed at children under 13.

## Contact

Questions about this policy: **balochscriptcom@gmail.com**
