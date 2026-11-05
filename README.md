# StreamAtlas updates

Current release: **1.4.8** (version code 36), Android 6 or newer.

- [32-bit ARM APK](https://gofile.io/d/S8pVdHJj)
- [64-bit ARM APK](https://gofile.io/d/DJPffkJp)

## Changes

- Guide date/time browsing of loaded schedules, with a Now shortcut. Compact phone layouts put the actions in the Guide menu. Past/future listings open details; streams remain live.
- Numeric TV tuning: enter up to five digits, then OK or a short wait. Back cancels, Delete edits, and navigation/pointer input cancels entry. Search fields retain numeric input. Android accessibility timing is respected.
- Both players and fullscreen browsing use global channel numbers without clearing filters. Playlist numbers are preferred; fallback numbers follow playlist order and can change after provider reordering.
- Improved large-text Guide layout and preserved sorted compatibility browsing order.

Users on 1.4.7 can use Settings > Check for app updates. Older builds need manual installation. The app checks [latest.json](latest.json) and selects a matching architecture. Android controls installation; the package/signing key are unchanged. Provider and schedule availability remain outside the app's control.

## Publishing a release

1. Build with a higher versionCode, the same package name and signing key.
2. Test and verify APK signatures, upload each APK and verify upload size/hash.
3. Update latest.json last with version code/name, minimum SDK, plain-text notes and verified HTTPS download pages. Keep the raw feed URL stable.

The feed holds public release information, not user watch history. File-host links may expire and can be replaced. GitHub raw-file caching can briefly retain the preceding manifest. Tests use injected fixtures rather than fictional public releases.
