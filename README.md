# StreamAtlas updates

Current release: **1.4.7** (version code 35), Android 6 or newer.

- [32-bit ARM APK](https://gofile.io/d/AHj8Ur9C)
- [64-bit ARM APK](https://gofile.io/d/QZrl5ExU)

This release adds continuing paced stream recovery, reconnection after internet/network changes, automatic update prompts and explicit TV Guide toolbar navigation. Stream availability still depends on the provider and network.

The app checks [latest.json](latest.json) for a newer compatible version and selects a matching architecture. Versions older than 1.4.7 require one manual installation to gain update checks. Installation remains controlled by Android; updates preserve the existing package and signing key.

## Publishing a release

1. Build with a higher versionCode, the same package name and signing key.
2. Test and verify APK signatures, upload each APK and verify upload size/hash.
3. Update latest.json last with the new code/name, minimum Android SDK, plain-text release notes and verified HTTPS download pages. Keep the raw manifest URL stable.

The feed holds public version information and links, not user watch history. File-host links may expire and can be replaced without changing the version. GitHub's raw-file cache may briefly retain a previous manifest after publishing. Never publish fictitious future versions for testing; tests use injected fixtures.
