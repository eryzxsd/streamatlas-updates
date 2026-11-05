# StreamAtlas updates

Current release: **1.4.9** (version code 37), Android 6 or newer.

- [32-bit ARM APK (TV and phone)](https://gofile.io/d/ONVH1Qoy)
- [64-bit ARM APK](https://gofile.io/d/GgJ40ZqX)

## Changes

- TV layouts reclaim space in Home, Channels, Guide, fullscreen browsing, search and Settings. The Settings form scrolls above fixed Save/Cancel buttons.
- Settings > Channel layout: logo grid adds logo tiles in Channels, Favorites and fullscreen browsing. Search, favorites and channel numbers are shared; Home and Guide keep their layouts.
- Numeric tuning is optional, enabled by default on TV. Show clock in fullscreen video is a separate option, off by default, and yields to controls and numeric entry.
- Future Guide/programme-search details offer reminders at start or five minutes before. Settings > Programme reminders manages them. Saving requests notification permission where required. Android may delay approximate alerts; precise timing access is optional. Notifications open details and require Watch live to tune.
- Playback engines, buffers, retries and EPG providers are unchanged.

Use Settings > Check for app updates. Builds older than 1.4.7 need manual installation. The app checks [latest.json](latest.json) and selects a matching architecture. Android controls installation; the package/signing key are unchanged. Provider and schedule availability remain outside the app's control.

## Publishing a release

1. Build with a higher versionCode, the same package name and signing key.
2. Test and verify APK signatures, upload each APK and verify upload size/hash.
3. Update latest.json last with version code/name, minimum SDK, plain-text notes and verified HTTPS download pages. Keep the raw feed URL stable.

The feed holds public release information, not user watch history. File-host links may expire and can be replaced. GitHub raw-file caching can briefly retain the preceding manifest. Tests use injected fixtures rather than fictional public releases.
