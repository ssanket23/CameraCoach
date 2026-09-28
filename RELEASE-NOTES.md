# CameraCoach 0.3.1 - early access

First public, release-signed Android distribution. Android 10 or newer.
Package: `com.cameracoach.app`; version code: `6`.

## Included

- Person + scenery, Portrait, and Scenery only coaching modes.
- Adjustable pose outlines and approximate live limb-direction feedback.
- Optional free Wikimedia Commons references with source/license attribution.
  Suitable downloaded photos create new pose geometry locally; this is not just a
  selection of built-in poses. No camera upload is used for reference search.
- Original-preserving capture, optional enhancement, and adjustable export crops.
- An expanded in-app privacy disclosure covering ML Kit SDK diagnostics.

## Known limitations

- Early prototype; broad device compatibility and sustained performance remain unverified.
- Pose analysis is intended for one roughly front-facing person with visible joints.
- Imported poses are restricted to confident upright full-body references.
- Background comparison uses broad categories, not exact visual similarity.
- Reference coverage varies. Empty results, download failures, and rate limits are possible.
- Reference photos are public and not curated; metadata filters are not a guarantee
  of audience suitability, rights clearance for other uses, or real-world safety.
- Zoom ratios do not guarantee switching a particular physical camera lens.
- No iOS version, automatic updates, accounts, ads, billing, or Play Store listing.
- ML Kit may send diagnostic/usage metrics even without a reference search.

## Installation and updates

Download the APK asset, not GitHub's automatically generated source archive.
Install only if you trust the publisher. Do not disable device security protections.
See the project page for installation and privacy information.

The dedicated release signing key differs from old development debug builds.
Do not expect an in-place update from those builds; preserve photos/settings before
choosing whether to uninstall a debug build. Later public releases will reuse this
release key and increment the version code.

The `.sha256` asset provides the APK hash. The signing-certificate asset contains only
the public certificate information, never the private signing key.

## Verification scope

The 0.3.0 debug prototype's core reference selection and scenery-only capture were
exercised on a Galaxy S23 FE, including live Commons retrieval and on-device extraction.
Version 0.3.1 adds release packaging and SDK privacy text, not new camera behavior.
The release passed 75 unit/Robolectric tests, Android lint, APK alignment, and
signature verification. Release-build details and the exact APK digest are attached
separately; prior debug device testing is not a claim that this signed release was
physically installed. Third-party notices and an exact dependency inventory are
included in the accompanying notices ZIP and distribution repository.
