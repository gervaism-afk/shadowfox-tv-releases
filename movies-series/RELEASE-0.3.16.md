# ShadowFoxTV Movies & Series 0.3.16

[Signed APK](ShadowFoxTV-Movies-Series-0.3.16.apk) · [Complete source](ShadowFoxTV-Movies-Series-0.3.16-source.zip) · [Updater feed](update.json) · [Verification](verification-0.3.16.json)

Movie/series detail and playback actions now share the ShadowFox Exclusive focus style: opaque charcoal surfaces, stable size, readable light text and a cyan focus outline. Cinema keeps its original button colors. Choose either look under Settings > Appearance; the choice persists.

The playback timeline has a 48dp touch target. Swipe horizontally to seek; the seek commits once at release and stays within the title. Cancelling a drag leaves playback alone. Tap still plays/pauses, and remote left/right/OK retain their existing behavior and acceleration. The timeline exposes current/total time and adjustable progress for accessibility. Portrait phones show a touch-specific hint.

Saved accounts, watch progress, continuous browsing, Adult shortcuts, phone portrait/rotation, TV landscape, touch controls, DTS audio and updater remain. Profiles/About remain absent from Settings. Adult titles still depend on provider categories; the tested account provides none. No new dependencies, player/decoder changes or database migrations.

Package `ca.shadowfoxtv.movieseries`, version code 28, Android 7.1/API 25 or newer. Install over your existing app to keep data. Signed with the original compatible certificate. Feed is separate from Platinum Player.

201 tests passed; release lint has no errors. Checks include swipe cancellation/clamping, no accidental play/pause, accessibility, remote focus and callbacks, and 320dp portrait layout. Actual player controls were rendered locally with a fixed clock and no media engine/network. The exact signed APK was installed/hash-verified on Tanix; movie/series detail focus and return position, retained theme/account/library and Updates were checked. No provider stream or physical phone playback was tested. The earlier Tanix 4K/heat issue remains unresolved.

Source includes Inter fonts/OFL licenses, AndroidX Media3/FFmpeg source, four-ABI audio libraries and provenance/licenses. Private keys and local configuration are excluded. Original attribution retained; AndroidX Media3 is Apache 2.0 and FFmpeg 6.1.6 LGPL 2.1 or later.
