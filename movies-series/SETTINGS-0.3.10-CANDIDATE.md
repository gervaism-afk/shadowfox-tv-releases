# Settings redesign — 0.3.10 candidate

Based on the published ShadowFoxTV Movies & Series 0.3.9 source archive.

Settings now has six categories: Account, Playback, Library, Profiles, Updates,
and About. Category controls and Back stay above the scrolling content.
Sections use consistent cards and controls fit the available width. On phones,
choice values sit below labels, input stays directly editable, action buttons
wrap, and the keyboard and system bars are accounted for. QR setup also wraps.

TV retains the deliberate OK-to-edit account dialog, masked passwords and
focus restoration after Done or Cancel. Focusing a category does not activate it.
The existing ViewModel retains unsaved account edits when changing categories.

Package ID and stored settings are unchanged. Candidate version: 0.3.10, code 22.
The published update feed remains on 0.3.9.

## Build and signing

Use JDK 17, Gradle 8.7, Android SDK 34 and build-tools 34.0.0. Run:

```sh
bash gradlew assembleDebug testDebugUnitTest --tests 'nl.vanvrouwerff.iptv.ui.settings.*' --tests 'nl.vanvrouwerff.iptv.data.settings.SourceSetupTest'
```

Apply settings-0.3.10.patch to the published 0.3.9 source archive to reproduce
this candidate. The public source excludes local.properties and signing keys. Local debug APKs
are for validation; they cannot update the official app. Recover the original
signing key and original TMDB configuration before publishing. Do not uninstall
the current app. Confirm the release certificate against the published 0.3.9 APK,
build and validate the release, and only then update the feed.

Official 0.3.9 signing certificate SHA-256:
`c018a048630b67d1b82a80308bb5e5c725fbbd7487eca6c0c461464884984e90`.
The saved debug key was checked and does not match this certificate.

## Verified locally

`assembleDebug` and all 10 selected interaction/account tests passed under JDK 17.
This includes 5 existing TV/phone editor/navigation tests, 2 new category and
narrow-phone tests, and 3 existing account-setup tests. Physical device testing
and official release signing are pending.
