# ShadowFoxTV Movies & Series 0.3.14

[Signed APK](ShadowFoxTV-Movies-Series-0.3.14.apk) · [Complete source checkpoint](ShadowFoxTV-Movies-Series-0.3.14-source.zip) · [Updater feed](update.json) · [Verification](verification-0.3.14.json)

Movies, Series, search and My List scroll continuously, with no Next/Previous page buttons. Small batches and a bounded paging cache keep large libraries responsive. Remote navigation has explicit paths between header, categories and titles. Returning from a title restores focus and position; returning from Settings retains the library position and focuses Settings. Search completion enters results. Phone touch remains supported.

Adult movies/series have a visible shortcut near the top of the library and category picker in ordinary profiles. Content depends on the provider supplying matching categories. If none are supplied, the section explains this. No titles are guessed or fabricated. Existing kids-profile filtering remains.

Settings has Account, Playback, Library and Updates. Profiles and About are absent from Settings. Stored accounts, profiles, watch progress, database schema, player, DTS audio support, updater and phone/TV orientation policy are retained. The Apple TV inspired interface is preserved.

Package `ca.shadowfoxtv.movieseries`, code 26, Android 7.1/API 25 or newer. Install over the existing app to retain your data. Signed with the original compatible certificate. This update feed is separate from Platinum Player.

187 automated tests passed; release lint has no errors. The exact final signed APK was installed and hash-verified on a Tanix TX68. Device checks covered continuous browsing beyond 60 titles, focus and position restoration, Settings and Adult shortcuts. The tested provider account supplies no Adult categories. No provider playback was initiated during these navigation checks. The earlier 4K reset/heat investigation remains unresolved.

The complete source includes AndroidX Media3/FFmpeg source, four-ABI audio libraries, provenance and licenses. Private signing keys and local configuration are excluded. Based on SERFF/iptv-app and AndroidX Media3 (Apache 2.0); FFmpeg 6.1.6 is used under LGPL 2.1 or later. Original attribution and LICENSE are retained.
