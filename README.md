# StreamAtlas updates

Public release metadata for StreamAtlas Android. Install the latest compatible APK through Android's installer; this repository does not change device settings.

The app checks [latest.json](latest.json) for a newer compatible version. Download URLs select 32-bit or 64-bit ARM according to the device. Older versions without update checks need one manual installation of v1.4.7 or newer.

## Publishing a release

1. Build with a higher versionCode, the same package name and signing key.
2. Test and verify APK signatures, then upload each APK and verify upload size/hash.
3. Update latest.json last with the new code/name, minimum Android SDK, plain-text release notes and verified HTTPS APK download pages. Keep the raw manifest URL stable.

The feed holds public version information and links, not user watch history. File-host links can expire and may be replaced without changing the version. Never publish fictitious future versions for testing; tests use injected fixtures.
