# ShadowFoxTV Movies & Series 0.3.28

[Signed APK](ShadowFoxTV-Movies-Series-0.3.28.apk) · [Complete source](ShadowFoxTV-Movies-Series-0.3.28-source.zip) · [Updater feed](update.json) · [Verification](verification-0.3.28.json)

Settings keeps the flat Launcher Pro format with a stronger visual hierarchy. Sharp section icons and a subtle rail divider make navigation easier to scan. Control names are larger than their descriptions, values align consistently, and TV switches show On/Off text. A soft focus fade retains the slim marker without scaling rows. Section introductions and theme descriptions use clearer copy; the selected theme has a checkmark. All controls keep their original focus order and callbacks.

Library refresh failures now show a readable title and guidance instead of a raw transport exception. The refresh backend is unchanged; this presentation change does not claim to fix provider connectivity. The original logo, saved-account storage, Adult visibility, player/database, updater backend, orientation, Home startup focus and editor caret/cancellation behavior are retained.

261 automated tests passed with zero failures, and release lint has zero errors. Existing tests cover TV remote navigation, small-screen scrolling, focus return, phone portrait/touch editing, editor selection/cancellation, password masking, themes, Adult visibility and updater behavior. TV and phone fixture screenshots were visually reviewed.

The original-signed APK was installed over 0.3.27 on Fire TV and the installed hash matched the download. Native checks opened the configured Home screen with Home focused, visited Appearance/Playback/Library/Updates, stopped at the final Playback row and restored the previous control when returning to Appearance. No real preference, refresh or playback action was activated. Appearance was left open for review. Fire TV is not rooted, so private preference files were not read or fingerprinted; Android's in-place update retained app data, and storage code is unchanged.

The user needed the Tanix for a game, so no Tanix input, install or app launch was performed in this pass. Only earlier read-only inventory preceded that coordination update. No startup, firmware, display or system changes were made. Provider playback and refresh connectivity were not tested.

Only the version and SettingsLayout, SettingsScreen and AppearanceSettings differ from 0.3.27. All resources are byte-identical, including the exact original logo. Package `ca.shadowfoxtv.movieseries`, version code 40, Android 7.1/API 25 or newer. Signed with the original compatible certificate. Install over the existing app to retain data. Complete source retains attribution, fonts, Media3/FFmpeg sources and licences; private keys and local configuration are excluded.
