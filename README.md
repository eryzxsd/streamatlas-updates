# StreamAtlas updates

Current release: **1.5.2** (version code 40), Android 6 or newer.

- [32-bit ARM APK (TV and phone)](https://gofile.io/d/nHLoQQSS)
- [64-bit ARM APK](https://gofile.io/d/kcmcYEIC)

## Changes

- Settings descriptions and helper text use smaller, secondary Material typography. Native controls and font scaling remain. The default Settings scrollbar is hidden while swipe and remote scrolling remain available.
- Closing PiP stops playback outside the app. Returning reopens that channel once after foreground resume and focus, including compatibility playback and custom streams. Pause, Stop, sleep expiry, focus loss and errors prevent unwanted recovery. Removed channels and changed playlists are discarded. Guide loading does not block recovery; expanding visible PiP keeps playing.
- The optional fullscreen clock uses tabular numerals, a compact Material surface and larger edge insets. It remains passive, follows the device time format and hides for controls, numeric tuning and PiP.

Use Settings > App > Check for app updates to fetch the matching architecture. Builds older than 1.4.7 need manual installation. Installation stays under Android/user control; package/signing key are unchanged.

Native libraries, decoder profiles, buffering, source retries and EPG providers are unchanged. Multiple playlists remain planned for later. Host verification does not certify physical-device playback or firmware behaviour.

## Publishing a release

1. Build with a higher versionCode, the same package name and signing key.
2. Test and verify APK signatures, upload each APK and verify upload size/hash.
3. Update latest.json with version code/name, minimum SDK, plain-text notes and verified HTTPS download pages. Keep the raw feed URL stable.

This feed holds public release information, not user watch history. File-host links may expire and can be replaced. GitHub raw caching may briefly retain the preceding manifest.
