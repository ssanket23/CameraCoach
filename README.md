# CameraCoach for Android

Free photography coaching, pose references, and optional photo enhancement.
**Early-access prototype, not a promise of professional results.**

- [Project page and installation instructions](https://ssanket23.github.io/CameraCoach/)
- [Download v0.3.1 APK](https://github.com/ssanket23/CameraCoach/releases/download/v0.3.1/CameraCoach-0.3.1.apk)
- [Release notes and checksums](https://github.com/ssanket23/CameraCoach/releases/tag/v0.3.1)
- [Privacy information](https://ssanket23.github.io/CameraCoach/#privacy)
- [Report an issue](https://github.com/ssanket23/CameraCoach/issues)

## What it does

- Live framing and phone-level guidance for a person or scenery.
- Pose outlines with user-selected styles, mirroring, size, and position controls.
- Optional free Wikimedia Commons search: locally derive a standing pose from a suitable photo.
- Dedicated Scenery only mode without person outlines.
- Capture an original, then optionally enhance and save a separate cropped copy.

**Android 10 or newer.** Current physical-device testing is limited to a Samsung Galaxy
S23 FE. There is no iPhone build, Play Store listing, subscription, or paid API account
required by this version.

## Install

1. Download `CameraCoach-0.3.1.apk` from the release linked above.
2. Open it on your Android phone. If Android requests permission, allow that browser or
   file app to install unknown apps, only if you trust this release. Revoke that
   installation permission afterward if you do not need it.
3. Open CameraCoach and allow camera access for live coaching, or choose Open photo
   to use the editor without camera permission.
4. Do not disable Play Protect or other security protections if installation is blocked.
   Managed devices and regional Android verification requirements may prevent sideloading.

There is no automatic updater. Download later releases from this repository and install
them over the existing release. Android will check the package and signing identity.
The first public release uses a dedicated signing key, different from earlier development
debug builds. Android cannot update those debug builds in place: preserve your photos and
any settings you need before choosing whether to uninstall a debug build yourself.

Use the accompanying `.sha256` file to check that a download matches the published APK.
This checks file integrity, not whether you trust the publisher. Signing-certificate
information is supplied in each release.

## Privacy and limitations

Camera and reference-image inference run on the phone. Optional Commons searches send
selected background keywords and ordinary connection information to Wikimedia; they
do not upload camera images or detected joints. Google ML Kit separately sends SDK
usage/diagnostic metrics to Google and may contact Google for configuration updates.
See the [full privacy information](https://ssanket23.github.io/CameraCoach/#privacy)
before installing. No separate CameraCoach analytics backend or advertising SDK is configured.

Pose/background suggestions are approximate. They are not safety assessments, exact scene
matching, gender identification, or photo-quality guarantees. Public reference results
are not curated; coverage varies and rate limits can interrupt searches. No app permission
grants access to your full photo library.

## Repository scope

This is a **download-only distribution repository**. It contains the project page,
privacy information, release documentation, and downloadable APK assets, not the app's
source code or signing credentials. GitHub's automatic "Source code" archive buttons
contain only these public site/documentation files.

CameraCoach is free to download and use; its app source is not offered under an
open-source license. Bundled dependencies and downloaded reference photos remain
subject to their respective licenses and notices. See [third-party notices](THIRD-PARTY-NOTICES.md).
No downloaded reference photo is bundled in the release or used as a marketing image.

For support, open a GitHub issue with the app version, Android version, and reproduction
steps. Issues are public: do not attach private photos, credentials, or sensitive logs.
