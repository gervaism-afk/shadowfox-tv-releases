# ShadowFoxTV Movies & Series 0.3.19

[Signed APK](ShadowFoxTV-Movies-Series-0.3.19.apk) · [Complete source](ShadowFoxTV-Movies-Series-0.3.19-source.zip) · [Updater feed](update.json) · [Verification](verification-0.3.19.json)

Home now has one continuous cinematic canvas. Wide featured artwork blends into the selected theme; the framed banner and duplicate floating poster are removed. Headings, actions and shelves align to one gutter. The primary action has a clear light fill, supporting actions are quieter, and shelf headings are simpler.

Continue Watching preserves full portrait artwork beside the title, caption and progress. Portraits are no longer cropped into landscape tiles. The shorter TV featured area leaves the first Continue card fully visible even on a 960x540 layout. Phones retain comfortable touch targets and scrolling; enlarged text expands the layout. Missing wide artwork uses a separate portrait fallback without inventing metadata.

Remote Down from the header returns to the featured primary action, including after deep shelf scrolling. Up from that action returns to Home. Existing detail-return shelf focus is retained. No automatic playback was introduced.

243 tests passed; release lint has no errors. New actual UI checks cover aligned gutters and a complete first Continue card on small TVs, both theme renders, header focus, correct Continue details callbacks, deep shelf return, missing artwork, narrow-phone touch and enlarged text. The exact signed APK was installed and hash-verified on Tanix; native Home layout, header movement, details/Back focus and installed version were checked. No provider stream was started or watch history edited. No physical-phone playback tested. Earlier Tanix 4K/heat issue remains unresolved.

Only the Home presentation file and app version changed from 0.3.18, with one new test file. The Home browse/data wrapper is unchanged. Account storage, recommendations and metadata providers, progress/database, series selection, player/native audio, phone orientation, library, Settings navigation and updater are byte-identical. Both Cinema and ShadowFox Exclusive remain available. Profiles/About remain absent from Settings. Adult content depends on provider-supplied categories.

Package `ca.shadowfoxtv.movieseries`, version code 31, Android 7.1/API 25 or newer. Install over the existing app to retain data. Signed with the original compatible certificate. This feed is separate from Platinum Player.

Complete source includes Inter/OFL fonts, AndroidX Media3/FFmpeg source, four-ABI audio libraries and licenses/provenance. Private signing keys and local configuration are excluded. Original attribution retained; AndroidX Media3 is Apache 2.0 and FFmpeg 6.1.6 LGPL 2.1 or later.
