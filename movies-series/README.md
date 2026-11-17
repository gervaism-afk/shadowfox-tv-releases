# ShadowFoxTV Movies & Series 0.3.18

[Signed APK](ShadowFoxTV-Movies-Series-0.3.18.apk) · [Complete source](ShadowFoxTV-Movies-Series-0.3.18-source.zip) · [Updater feed](update.json) · [Verification](verification-0.3.18.json)

Series Play/Continue now defaults to the first playable main season, with Specials after the main seasons. Generic Season 0 labels read Specials; custom provider names are preserved. Specials-only shows remain playable, and an intentional in-progress special still resumes. Completing the main series does not send the primary action into unstarted specials.

After a finished episode, the primary action skips watched following episodes and retains a saved resume point in its next choice. Obsolete episode IDs no longer hide a valid resume. Saved watch history is read without rewriting it. Playback ordering is prepared once per series load instead of being sorted on every progress update. These changes affect the series detail Play/Continue choice; player cross-season autoplay is unchanged.

235 tests passed; release lint has no errors. New checks cover main/special ordering, resume preservation, watched/empty/specials-only cases, threshold boundaries, stale progress, unchanged history, actual primary-button payloads, loading focus, remote season selection and phone touch. TV/phone components were rendered locally without a media engine. The exact signed APK was installed and hash-verified on Tanix. The same untouched Percy Jackson case changed from Play S0:E1 to Play S1:E1; Season 1/Season 2/Specials order, manual Specials selection, detail Back focus and installed version were checked. No provider stream was started or history edited. No physical phone playback was tested. Earlier Tanix 4K/heat issue remains unresolved.

Settings navigation from 0.3.17, both themes, saved accounts/progress, continuous scrolling, Adult shortcuts, phone rotation, TV landscape, touch controls, DTS audio and updater are retained. Profiles/About remain absent from Settings. Provider content still depends on supplied categories. No database migration or account/player/decoder changes. Series network/auth/cache and active-profile progress subscription behavior are retained; primary-button extraction preserves its callback and layout.

Package `ca.shadowfoxtv.movieseries`, version code 30, Android 7.1/API 25 or newer. Install over the existing app to retain data. Signed with the original compatible certificate. This feed is separate from Platinum Player.

Complete source includes Inter/OFL fonts, AndroidX Media3/FFmpeg source, four-ABI audio libraries and licenses/provenance. Private signing keys and local configuration are excluded. Original attribution retained; AndroidX Media3 is Apache 2.0 and FFmpeg 6.1.6 LGPL 2.1 or later.
