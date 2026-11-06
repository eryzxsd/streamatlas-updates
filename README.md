# StreamAtlas updates

Current release: **1.6.0** (version code43), Android 6 or newer.

- [32-bit ARM APK (TV and phone)](https://github.com/eryzxsd/streamatlas-updates/releases/download/v1.6.0/StreamAtlas-1.6.0-armv7.apk)
- [64-bit ARM APK](https://github.com/eryzxsd/streamatlas-updates/releases/download/v1.6.0/StreamAtlas-1.6.0-arm64.apk)
- [Release notes](https://github.com/eryzxsd/streamatlas-updates/releases/tag/v1.6.0)

Save multiple playlists: merge enabled sources by default, or switch to a single playlist. Add optional Free-TV, Australia/Sydney and New Zealand presets.

IPTV-EPG country guides merge with existing guides by default. All 67 published countries are selectable; automatic loading fetches countries identified in enabled channel IDs. Existing schedules take priority. EPG coverage requires matching IDs. Country/provider switches and custom XMLTV sources are available in Settings > Sources > Playlists & guides.

Guide data appears progressively, with per-source caching and saved-guide fallback. New source identities are preserved through favourites, PiP and compatibility browsing.

Restores automatic foreground update checking on mobile and TV and adds Cancel/Exit confirmation at the app root. Existing playback engines and native libraries are retained.

Existing installations may need one manual update check to install the corrected automatic-check policy. Both APKs retain package org.streamatlas.player.debug and the existing signing key.

This repository holds release APKs and metadata, not viewer watch history. Country source availability and matching IDs determine EPG coverage.

