# StreamAtlas updates

Current release: **1.5.0** (version code 38), Android 6 or newer.

- [32-bit ARM APK (TV and phone)](https://gofile.io/d/B6abdAT5)
- [64-bit ARM APK](https://gofile.io/d/e5CkzyRR)

## Changes

- Settings and the contents of Home Search use Google's provided Material components and existing app theme. Settings groups Playback, Channels, Sources and App, retains drafts across tabs and keeps Save/Cancel outside scrolling content.
- Independent video decoding choices: normal Auto/HW/SW; compatibility Auto/HW/HW+/SW. Normal HW prefers hardware with decoder fallback; SW uses available Android software video codecs. Compatibility HW disables direct rendering; HW+ requests forced hardware/direct rendering with VLC fallback. Auto remains the default. Normal changes apply when reopening a channel; the compatibility in-player chooser reconnects immediately.
- Play in background and Picture-in-picture are separate menu actions and automatic options. Background defaults off. Both automatic options prefer PiP; explicitly choosing background skips PiP for that departure. Pause/Stop and sleep timers remain respected.
- Guide always shows current/next. Date & time and Now controls were removed, including overflow versions; full schedules and future reminders remain.
- Multiple playlists are planned for a later update and are not shipped in this version.

Use Check for app updates in Settings (App tab in the new Settings). Builds older than 1.4.7 need manual installation. The app reads [latest.json](latest.json) and selects the matching architecture. Android controls installation; package/signing key are unchanged. Stream and schedule availability depend on their sources. Host tests do not certify physical-device codec performance.

## Publishing a release

1. Build with a higher versionCode, the same package name and signing key.
2. Test and verify APK signatures, upload each APK and verify upload size/hash.
3. Update latest.json with version code/name, minimum SDK, plain-text notes and verified HTTPS download pages. Keep the raw feed URL stable.

This feed holds public release information, not user watch history. File-host links may expire and can be replaced. GitHub raw caching may briefly retain the preceding manifest.
