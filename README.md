# StreamAtlas updates

Current release: **1.5.4** (version code 42), Android 6 or newer.

- [32-bit ARM APK (TV and phone)](https://github.com/eryzxsd/streamatlas-updates/releases/download/v1.5.4/StreamAtlas-1.5.4-armv7.apk)
- [64-bit ARM APK](https://github.com/eryzxsd/streamatlas-updates/releases/download/v1.5.4/StreamAtlas-1.5.4-arm64.apk)
- [Release notes](https://github.com/eryzxsd/streamatlas-updates/releases/tag/v1.5.4)

## Changes

- Fullscreen and PiP video no longer retain the inline PlayerView rounded background/clipping outline, removing extra mobile video corner marks. Inline styling returns on exit.
- Sources URL fields use one Material label and an independent placeholder. Large-font URL examples remain on one line with end ellipsis. XML/.XML.GZ support is supporting text below the guide field.

34 targeted host tests across six suites passed. APK assembly and lint passed with zero errors (107 warnings). Signatures/package identity and unchanged native library bytes verified. Native phone/TV/200% text fixtures inspected; these do not certify physical-device SurfaceView/decoder behavior.

Use Settings > App > Check for app updates. Version 1.5.3 supports downloading this release inside the app with progress, cancellation/retry and verified installation. Earlier builds open their browser once. Android may require allowing installation from StreamAtlas and always controls the install step. Package/signing key are unchanged, so updating preserves app data.

Guide ordering, fullscreen categories/Favorites/Recent, numeric tuning preferences and the player-bar fullscreen control remain available. Playback engines, buffering, EPG providers and the direct-update downloader are unchanged. Multiple playlists remain planned for later.

## Publishing a release

1. Build a higher versionCode with the same package and signing key.
2. Verify tests/signatures, upload matching ARM APKs to GitHub Releases, and verify asset size/SHA-256 and public download URLs.
3. Update latest.json with version/minimum SDK/notes, HTTPS downloads, and directDownloads objects containing url/sha256/size per ABI. Keep the raw feed URL stable.

This repository holds public APKs and metadata, not user watch history. GitHub raw caching can briefly retain the preceding manifest.
