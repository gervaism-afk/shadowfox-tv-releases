# ShadowFoxTV Movies & Series 0.3.20

[Signed APK](ShadowFoxTV-Movies-Series-0.3.20.apk) · [Complete source](ShadowFoxTV-Movies-Series-0.3.20-source.zip) · [Updater feed](update.json) · [Verification](verification-0.3.20.json)

Go to **Settings > Library > Show Adult categories**. Turn it off to hide Adult shortcuts, provider categories and their titles from Movies, Series, category pickers, search, My List and Home, including Continue Watching. Turn it on to restore provider-supplied content. Changes save automatically, apply without a manual refresh and persist after restarting. Existing installs default to shown to preserve their previous visibility. Saved favourites and watch history are filtered without being deleted.

Hiding an open Adult category returns to All titles while preserving the media type, search and saved filter. Initial library visibility waits for the stored preference. Existing kids restrictions still hide Adult categories even if the switch is on; no profile selector or PIN prompt was added. This option uses the existing provider-category matcher (Adult, XXX, 18+, porn); it does not infer ratings or create content absent from your provider.

The whole Settings row works with remote OK or phone touch and exposes its checked state for accessibility. It is the first Library control, before Refresh, with the existing ordered remote focus and Back paths.

254 tests passed; release lint has no errors. Eleven new tests cover saved preference/default/account-theme-history-key preservation, restriction policy, reactive counts/categories, stale Adult selection, first-load preference gating, real Room paging/search/favourites/Home discovery hide/unhide without deletion, TV remote focus, phone touch and category-picker visibility with supplied or missing Adult categories. The exact signed APK was installed in place and hash-verified on Tanix. Native toggle, Movies/Series/picker shortcuts, restart persistence and installed version were verified. This account supplies no Adult categories, so title-level filtering used database fixtures. No provider stream or physical-phone playback tested. Earlier Tanix 4K/heat issue remains unresolved.

The 0.3.19 Home redesign, both themes, saved account credentials, history, continuous paging, phone rotation, TV landscape, touch, series Play/Continue, player/native DTS audio, Settings navigation and updater are retained. No database schema, catalogue-import/authentication, player or updater changes. One stored visibility key and the new filtering connections were added; no account or history migration.

Package `ca.shadowfoxtv.movieseries`, version code 32, Android 7.1/API 25 or newer. Install over the existing app to retain data. Signed with the original compatible certificate. This feed is separate from Platinum Player.

Complete source includes Inter/OFL fonts, AndroidX Media3/FFmpeg source, four-ABI audio libraries and licenses/provenance. Private signing keys and local configuration are excluded. Original attribution retained; AndroidX Media3 is Apache 2.0 and FFmpeg 6.1.6 LGPL 2.1 or later.
