# ShadowFoxTV Movies & Series v0.2.8

[Download single APK](ShadowFoxTV-Movies-Series-0.2.8.apk) · [Source ZIP](ShadowFoxTV-Movies-Series-0.2.8-source.zip) · [Updater feed](update.json) · [Verification](verification-v0.2.8.json)

Fixes TV remote search losing typed text and caret position. Movies search stays within movies, and Series search stays within series. Episode lists now tolerate blank optional provider metadata. Playback recovers automatically when a provider advertises an HLS playlist but returns an MKV/MP4 video file.

Verified on H96 Max: the previously failing Chicago Med S12E01 produced video frames, selected audio and advancing playback. All 112 unit tests pass. Genuine empty or unavailable provider listings can still have no episodes.

Package `ca.shadowfoxtv.movieseries`, version code 10. Install over the existing app to retain login and library. Existing updater users can use Settings > App updates. Android 7.1/API 25 and newer; includes 32-bit ARM libraries and mobile/TV launchers. Fire OS 6 compatibility retained; physical Firestick playback still requires confirmation. v0.2.0 users need one manual bootstrap update.

Final artwork and database schema 18 are retained. Source excludes private signing keys and local machine settings. Official updates require the privately retained compatible signing key.

Source based on SERFF/iptv-app (Apache 2.0); original attribution and LICENSE retained. This updater feed is isolated from Platinum Player.
