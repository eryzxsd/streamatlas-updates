# StreamAtlas updates

Current release: **1.5.3** (version code 41), Android 6 or newer.

- [32-bit ARM APK (TV and phone)](https://github.com/eryzxsd/streamatlas-updates/releases/download/v1.5.3/StreamAtlas-1.5.3-armv7.apk)
- [64-bit ARM APK](https://github.com/eryzxsd/streamatlas-updates/releases/download/v1.5.3/StreamAtlas-1.5.3-arm64.apk)
- [Release notes and APKs](https://github.com/eryzxsd/streamatlas-updates/releases/tag/v1.5.3)

## Changes

- Guide puts current/upcoming programme coverage first, preserving order within covered and uncovered groups and retaining scrolled anchors.
- Fullscreen browsing adds All, Favorites, Recent and categories. Search stays shared. Recent follows playback order. Disabling numeric tuning hides both input overlays and channel-number prefixes. The floating fullscreen shortcut no longer appears when video controls hide; the bar retains fullscreen and compact mini-player expansion remains accessible.
- Direct APK downloads run through Android DownloadManager, with percentage/byte progress, Hide, Cancel and Retry. Size, SHA-256, package, version and current signing certificate must match before Install becomes available. Android retains control of installation; allowing updates from StreamAtlas may be required.
- Compatibility HW/HW+ labels now explain VLC decoding-only versus decoding plus direct rendering. Explicit HW follows official VLC options. These are VLC modes, not a copy of MX Player's proprietary framework. Auto, SW, normal Media3 selection and native libraries remain unchanged.

Use Settings > App > Check for app updates. Existing older builds open the browser once to install 1.5.3; later direct releases can download inside the updated app. The feed selects a supported system ABI. Package/signing key are unchanged, so updating preserves app data. Downloads are now hosted on GitHub Releases.

129 targeted host checks across 17 suites passed; assembly and lint passed with zero errors (107 warnings). All APK signatures and unchanged native library bytes verified. Uploaded GitHub asset sizes/SHA-256 match local signed files. Native phone/TV/large-text samples inspected; no physical-device playback or installer verification is claimed. Multiple playlists remain planned for later.

## Publishing a release

1. Build a higher versionCode with the same package and signing key.
2. Test, verify signatures, upload matching ARM APKs to GitHub Releases and verify uploaded size/SHA-256 and public URLs.
3. Update latest.json with version code/name, minimum SDK, notes, HTTPS downloads, and directDownloads objects containing url/sha256/size per ABI. Keep the raw feed URL stable. Older apps ignore directDownloads and use downloads in their browser.

This repository holds public release metadata and APKs, not user watch history. Installation remains an explicit Android/user action. GitHub raw caching can briefly retain the preceding manifest.
