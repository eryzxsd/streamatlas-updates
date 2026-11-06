# StreamAtlas updates

Current release: **1.5.1** (version code 39), Android 6 or newer.

- [32-bit ARM APK (TV and phone)](https://gofile.io/d/JZxf5tv3)
- [64-bit ARM APK](https://gofile.io/d/JDxVxuCR)

## Changes

- Closing PiP stops playback, clears background/resume/retry intent and removes notification controls, even with automatic background playback enabled. Expanding visible PiP keeps playing. Compatibility closure follows the existing isolated-process exit path without synchronous native stop on the UI thread.
- Guide details and update availability now use provided Material typography, dividers and standard action buttons. Status/coverage lead Guide details; long URLs and release notes scroll above fixed actions.
- Compatibility playback now checks for automatic updates too. Unacknowledged available results can be rechecked after activity/process loss. Failed/incomplete checks become eligible after five minutes; successful no-update checks retain twelve hours. Checks run at startup/check events, not as continuous polling. Explicit interrupted close permits recheck.
- Later postpones the same version for24h; successful Download acknowledgement is shared for12h between players. Manual checks bypass acknowledgement delays.

If the existing phone build misses the automatic prompt, use Settings > App > Check for app updates once to install this fix. Builds older than1.4.7 need manual installation. The app reads [latest.json](latest.json) and selects the matching architecture. Installation stays under Android/user control; package/signing key are unchanged.

Decoder profiles, buffering, source retries and EPG providers are unchanged. Multiple playlists remain planned for a later update. Host verification does not certify physical-device decoding or firmware behaviour.

## Publishing a release

1. Build with a higher versionCode, the same package name and signing key.
2. Test and verify APK signatures, upload each APK and verify upload size/hash.
3. Update latest.json with version code/name, minimum SDK, plain-text notes and verified HTTPS download pages. Keep the raw feed URL stable.

This feed holds public release information, not user watch history. File-host links may expire and can be replaced. GitHub raw caching may briefly retain the preceding manifest.
