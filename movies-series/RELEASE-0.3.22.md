# ShadowFoxTV Movies & Series 0.3.22

[Signed APK](ShadowFoxTV-Movies-Series-0.3.22.apk) · [Complete source](ShadowFoxTV-Movies-Series-0.3.22-source.zip) · [Updater feed](update.json) · [Verification](verification-0.3.22.json)

The shared Home, Movies, Series, My List and Search header now uses an outlined Settings gear. It retains the Settings accessibility label, focus outline and existing navigation callback, with a 48dp target and the same TV header height.

Inside the app, the small raster badge has been replaced with a clean orange/navy/white fox vector and live brand lettering. The mark scales with display density instead of enlarging the old 80dp bitmap assets. Header, welcome, loading, legacy browse header and Home fallback branding all use the scalable mark. The loading screen renders ShadowFoxTV and MOVIES & SERIES as text. Android 12's system startup uses an inset vector too. Launcher icons, round icons and TV banners are unchanged, as requested.

254 existing automated checks passed; release lint has no errors. The phone Settings check verifies the accessible gear, minimum touch size and callback. Both theme/TV/phone previews were reviewed. The exact signed APK was installed and hash-verified on Tanix; new Home/library branding, gear focus, opening Settings and Back to the same gear bounds, the Adult visibility control and installed version were checked. Android 12 startup resources compiled; no physical-phone startup/playback was tested. No preferences were edited or provider playback started.

Only seven existing files changed from public 0.3.20: app version, shared header, four other in-app logo surfaces and the necessary phone test selector. Three new XML resources provide the vector mark and Android 12 startup presentation. The navigation callbacks/focus requesters, saved logins, Adult visibility, history, both themes, Home layout, continuous paging, player/native audio, orientation, database and updater are unchanged. 0.3.21 was an internal gear-only checkpoint and was not published. Earlier Tanix 4K/heat issue remains unresolved; no playback or thermal changes are claimed.

Package `ca.shadowfoxtv.movieseries`, version code 34, Android 7.1/API 25 or newer. Install over the existing app to retain data. Signed with the original compatible certificate. This feed is separate from Platinum Player.

Complete source includes Inter/OFL fonts, AndroidX Media3/FFmpeg source, four-ABI audio libraries and licenses/provenance. Private signing keys and local configuration are excluded. Original attribution retained; AndroidX Media3 is Apache 2.0 and FFmpeg 6.1.6 LGPL 2.1 or later.
