# ShadowFoxTV Movies & Series 0.3.26

[Signed APK](ShadowFoxTV-Movies-Series-0.3.26.apk) · [Complete source](ShadowFoxTV-Movies-Series-0.3.26-source.zip) · [Updater feed](update.json) · [Verification](verification-0.3.26.json)

On TV startup, remote focus now lands on the top Home button. Reopening the existing Home screen from the launcher requests Home focus again. Moving Right focuses Movies, and loading new Home data keeps that focus. Returning from a title retains the existing tile restoration; opening another screen does not continuously reset focus. Phone touch behavior is unchanged.

The signed release was installed over the previous app on Tanix TX68. Cold launch focused Home without any navigation input. Right focused Movies and remained there after loading; an ACTION_MAIN launcher reopen focused Home again. The installed APK matches the download hash, and the complete saved-preferences fingerprint was unchanged. The box was left on Home with Home focused. No playback or Fire TV commands were issued, and no startup, display or system setting was modified.

261 automated tests passed with zero failures. Release lint has zero errors. Regression checks cover initial Home focus, Right navigation, loading updates, launcher-reopen focus, existing deep-shelf return focus, phone portrait/touch and settings editing/navigation.

Only the version, MainActivity launcher callback, Home view model, Home screen and Home presentation test differ from 0.3.25. Original logo/artwork, account storage, category filters, Adult visibility, player, database, orientation and verified updater remain unchanged. Fire TV can obtain the release through the updater; it was not directly updated in this pass. No provider playback was tested.

Package `ca.shadowfoxtv.movieseries`, version code 38, Android 7.1/API 25 or newer. Signed with the original compatible certificate. Install over the existing app to retain data. Complete source retains attribution, Inter/OFL fonts, Media3/FFmpeg sources and licences. Private signing keys and local configuration are excluded.
