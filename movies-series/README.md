# ShadowFoxTV Movies & Series v0.2.9

[Download single APK](ShadowFoxTV-Movies-Series-0.2.9.apk) · [Source ZIP](ShadowFoxTV-Movies-Series-0.2.9-source.zip) · [Updater feed](update.json) · [Verification](verification-v0.2.9.json)

Movies and Series each keep six recent searches per profile, newest first, without case-insensitive duplicates. Finish a search with the keyboard Search key, close the keyboard, select a title, close Search or switch sections to save it. Recent search buttons beneath the bar recall the complete query. Clear history affects only the current section; the X in the bar clears the current text. History survives app restarts.

While the keyboard is open, smaller complete posters use the full width above it. Navigation, category sidebar and history return when it closes. H96 window-visibility quirks are handled using the actual unobscured window height. Verified on the physical H96; all 117 tests pass.

Includes v0.2.8 fixes for TV search text/caret, separate movie/series result scopes, blank optional provider episode metadata, and video files mislabeled as HLS playlists. Provider availability and codec support can still affect individual titles.

Package `ca.shadowfoxtv.movieseries`, version code 11. Install over the existing app to retain login and library. Existing updater users can use Settings > App updates. Android 7.1/API 25 and newer; includes 32-bit ARM libraries and mobile/TV launchers. Fire OS 6 compatibility retained; physical Firestick playback still requires confirmation. v0.2.0 users need one manual bootstrap update.

Final artwork and database schema 18 are retained. Source excludes private signing keys and local machine settings. Official updates require the privately retained compatible signing key.

Source based on SERFF/iptv-app (Apache 2.0); original attribution and LICENSE retained. This updater feed is isolated from Platinum Player.
