# StreamAtlas updates

Current release: **1.6.1** (version code44), Android 6 or newer.

- [32-bit ARM APK (TV and phone)](https://github.com/eryzxsd/streamatlas-updates/releases/download/v1.6.1/StreamAtlas-1.6.1-armv7.apk)
- [64-bit ARM APK](https://github.com/eryzxsd/streamatlas-updates/releases/download/v1.6.1/StreamAtlas-1.6.1-arm64.apk)
- [Release notes](https://github.com/eryzxsd/streamatlas-updates/releases/tag/v1.6.1)

Playlist loading, saved source management and M3U parsing now use Kotlin. XMLTV parsing, merged EPG loading and guide-cache handoff also use Kotlin.

Preserves the current Google Material interface, mobile/TV player controls, playback engines and guide providers. Existing playlist settings, channel IDs, favourites and cache formats remain compatible.

Retains background loading ownership, cancellation, cached fallback and progressive guide results. Kotlin is the project default for future features and UI work.

Settings > App > Check for app updates installs this release through the existing update flow. The current multiple-playlist merge/single views, optional free playlist presets and automatic IPTV-EPG country merging remain available. Guide coverage depends on matching XMLTV IDs.

This repository holds release APKs and metadata, not viewer watch history.

