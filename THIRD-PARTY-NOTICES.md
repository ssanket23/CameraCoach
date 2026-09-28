# Third-party notices

CameraCoach's app source is not published in this distribution repository.
Third-party components retain their own licenses. The notes below do not replace
the applicable upstream terms or any notices packaged inside the APK.

## AndroidX

The app uses AndroidX Activity, Core, CameraX camera-camera2, camera-lifecycle,
camera-view, and camera-mlkit-vision, with supporting transitive AndroidX components.

- Copyright: The Android Open Source Project / respective component contributors.
- License: Apache License, Version 2.0.
- Source and license information: https://android.googlesource.com/platform/frameworks/support/
- License text: [LICENSE-APACHE-2.0.txt](LICENSE-APACHE-2.0.txt).
- CameraX dependencies are version 1.5.3; Activity 1.10.1 and Core 1.16.0.

## Google ML Kit and Google/Firebase runtime components

The app bundles ML Kit pose detection 18.0.0-beta5 and image labeling 17.0.9,
along with their Google/Firebase runtime dependencies. These SDKs are not represented
as CameraCoach-owned or uniformly Apache-licensed software.

- ML Kit terms and privacy: https://developers.google.com/ml-kit/terms
- ML Kit Android data disclosures: https://developers.google.com/ml-kit/android-data-disclosure
- Google APIs terms: https://developers.google.com/terms
- Firebase Android open-source components and notices: https://github.com/firebase/firebase-android-sdk
- Google Tasks documentation: https://developers.google.com/android/guides/tasks

Input images and inference outputs are processed on-device. Google SDK diagnostic,
usage, installation, and configuration traffic is separately disclosed in the privacy page.
Google names and marks belong to their respective owners. No endorsement is implied.

## Other bundled open-source components

The resolved release runtime includes Kotlin standard library/coroutines, Guava's
ListenableFuture, OkHttp, Okio, Java injection annotations, and Google
transport/encoding components. Vendor SDKs also contain bundled third-party code.
Their upstream copyright and license notices apply:

- Kotlin: https://github.com/JetBrains/kotlin (Apache-2.0).
- Kotlin coroutines: https://github.com/Kotlin/kotlinx.coroutines (Apache-2.0).
- Guava: https://github.com/google/guava (Apache-2.0).
- Protocol Buffers: https://github.com/protocolbuffers/protobuf (BSD-3-Clause).
- Firebase Android SDK components: https://github.com/firebase/firebase-android-sdk (Apache-2.0).
- OkHttp: https://github.com/square/okhttp (Apache-2.0).
- Okio: https://github.com/square/okio (Apache-2.0).
- Java injection annotations: https://github.com/javax-inject/javax-inject (Apache-2.0).

See [DEPENDENCIES.json](DEPENDENCIES.json) for all 86 unique resolved runtime
component versions, license declarations from their POMs, and links to the original
notice files extracted from those artifacts and their nested JARs.
The [third-party-licenses](third-party-licenses/) directory retains those files
unchanged, including Google's bundled third-party license text and attribution
indexes. Identical files are deduplicated by SHA-256, not rewritten.
An empty POM license list means that the immediate POM did not declare a license;
it does not mean that a component is unlicensed or public domain.
AndroidX Camera Core's included notice also contains its BSD notices.
Some Google binaries use their vendor terms instead of an open-source license.
The release's third-party-notices ZIP includes this inventory and these license files.

## Wikimedia Commons references

No Commons reference photo is bundled in the APK or the project website.
When the user explicitly searches, eligible photos are downloaded temporarily from
Wikimedia Commons. In-app cards identify the creator, available credit/attribution,
source page, and license. Supported metadata includes public domain, CC0, CC BY,
and CC BY-SA. Imported outlines adapt detected joint directions into standard
mannequin proportions and are presented under the reference's license.

License metadata does not automatically clear privacy, personality, trademark, or
other rights. There is no endorsement by the people in reference photos or by Wikimedia.
The app does not include reference photos in captured images or export them to the gallery.
