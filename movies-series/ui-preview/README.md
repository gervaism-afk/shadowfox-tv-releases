# ShadowFoxTV Movies & Series 0.3.0 UI preview

[Download signed APK](https://raw.githubusercontent.com/gervaism-afk/shadowfox-tv-releases/movies-series-ui-preview/movies-series/ui-preview/ShadowFoxTV-Movies-Series-0.3.0.apk)

Apple TV-inspired dark Home, featured title, bounded horizontal Continue Watching, My List, Movies and Series rows, neutral white focus, touch and D-pad navigation. Based on tested v0.2.9; scoped search histories and playback fixes retained.

Install over the existing Movies & Series app; package and signer are unchanged. Do not uninstall. Requires Android 7.1/API25 or newer. This is a preview, with no physical H96/Fire TV test yet. Stable feed stays v0.2.9; Platinum Player is untouched.

APK SHA-256: 108bbf50f8198364a834cd6cf4273f2960255a6305217baeed7fa63e8419875f

121 tests pass. Release build, vital lint, APK signature and embedded PNG retention pass. Full lint reports one existing Media3 opt-in issue in unchanged StreamFormatRecovery.kt. Headless screenshot capture is unavailable; touch and D-pad UI assertions pass. [Verification](verification-v0.3.0.json).

## Source

[Complete source checkpoint](https://raw.githubusercontent.com/gervaism-afk/shadowfox-tv-releases/movies-series-ui-preview/movies-series/ui-preview/ShadowFoxTV-Movies-Series-0.3.0-source-checkpoint.zip); SHA-256 3b0275dfea752e8ead6230ea8c2b8b32304170c47c60a19869bc85eddb3363d5. Production source is exactly the code used for this APK. Extract, then apply [ci-fixes.patch](ci-fixes.patch) from the project root with `git apply` for the final test and build configuration: corrected Android test qualifier order, screenshot capture removed from the navigation regression gate, lower-memory single-worker build. All 121 tests then pass. Private key/local settings/build outputs are excluded. Supply the original compatible signing key privately at `signing/preview-debug.keystore`; do not generate a replacement key for an update build.
