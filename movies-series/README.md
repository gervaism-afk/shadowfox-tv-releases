# ShadowFoxTV Movies & Series 0.3.27

[Signed APK](ShadowFoxTV-Movies-Series-0.3.27.apk) · [Complete source](ShadowFoxTV-Movies-Series-0.3.27-source.zip) · [Updater feed](update.json) · [Verification](verification-0.3.27.json)

Settings now follows the user-approved Launcher Pro flat style. Section headings, simple rows, dividers and a slim focus marker replace the nested boxes. The style covers Account, Appearance, Playback, Library, Updates, informational panels and editor actions. Theme choices retain their colour previews and selected state. The settings update center uses unboxed version/status information; the separate update prompt keeps its previous appearance.

Existing remote navigation and touch behavior are retained. Up/Down traverses ordered controls, Left returns to the section list, and reentering a section restores its last control. Passwords stay masked, OK opens account editors, the cursor starts at the end, Cancel discards edits and restores focus, and saved preferences remain unchanged. The top Home startup focus from 0.3.26 is retained.

261 automated tests passed with zero failures; release lint has zero errors. Existing checks cover TV navigation and scrolling, small-TV bounds, editor cursor/cancellation, password masking, phone portrait/direct editing, themes, Adult visibility and updater behavior. Fixture screenshots were visually reviewed.

The original-signed APK was installed in place on Tanix TX68 and its installed hash matched the download. Native checks visited Appearance, Playback, Library and Updates without activating real settings or playback. Scrolling stopped at the final Playback row; section return restored the previous theme control. The real category-filter keyboard opened at the end of the saved value and Cancel restored its row. The entire saved-preferences fingerprint matched the previously verified 0.3.26 installation. Appearance was left visible for review. No Fire TV commands or startup/system/display changes were made. The foreground guard stopped input when the launcher appeared; the editor check resumed only after the user confirmed the box was free.

Library displayed a network refresh error (`stream was reset: INTERNAL_ERROR`). No manual library refresh was started in these checks, and provider connectivity/playback was not validated. This settings presentation update does not claim to resolve that network error.

Only the version and five presentation files differ from 0.3.26. Original artwork/resources, account storage, filters/Adult preference, playback backend, database, orientation, Home focus and verified updater backend remain unchanged. No provider playback was tested. Fire TV was not directly updated in this pass; it can obtain the signed release through its normal updater.

Package `ca.shadowfoxtv.movieseries`, version code 39, Android 7.1/API 25 or newer. Signed with the original compatible certificate. Install over the existing app to retain data. Complete source retains attribution, Inter/OFL fonts, Media3/FFmpeg sources and licences; private keys and local configuration are excluded.
