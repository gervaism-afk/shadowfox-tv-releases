# ShadowFoxTV Movies & Series 0.3.31

[Signed APK](ShadowFoxTV-Movies-Series-0.3.31.apk) · [Source](ShadowFoxTV-Movies-Series-0.3.31-source.zip) · [Updater feed](update.json) · [Verification](verification-0.3.31.json)

Selecting Home from the library in 0.3.30 could leave the screen without a focused
control. This update gives explicit Home and Back actions a single Home focus request.
Settings opened from Home returns to its gear; featured-title details return to the
primary action. Shelf details still restore the original poster and scroll position.
Warm launcher/Home requests override stale detail return targets. These are transient,
one-shot navigation intents: artwork, metadata and catalogue emissions do not steal
focus, and phone layouts do not receive TV focus requests.

Includes the complete 0.3.30 presentation: vector Home actions, full-collection shelf
links, visible detail Back controls, clearer search/loading/empty states, consistent
primary controls and the latest Settings theme samples/grouping/status/editors.

279 tests passed with zero failures; release lint has zero errors. New
checks exercise visible Home focus and the next Right press after a library return,
gear/primary returns without playback, no focus stealing after data updates, phone
focus gating, one-shot poster/header intent and warm-launch override. Existing Home,
detail, paging, Settings, saved-account, Adult, orientation and updater tests passed.

The 0.3.30 defect was reproduced on the user's free Fire TV. The original-signed 0.3.31
update was installed in place, and the installed APK hash matches this download.
Native checks passed cold Home focus, Home/header and hardware Back library returns,
Settings-to-gear return, featured-detail primary return and original shelf-poster
restoration. No app data was cleared and the configured catalogue loaded. No real
preference, manual test/refresh or provider-playback action was activated; audio,
system/display, server/key settings and other devices were untouched. Private account
files were not read. Provider connectivity/playback/audio were not validated.

Only version, HomeScreen and HomeViewModel change from 0.3.30; the new transient focus
controller and two regression test files are added. All resources including the exact
original logo, account storage/schema, database, Settings/player, updater backend and
orientation files remain byte-identical. Package `ca.shadowfoxtv.movieseries`, code 43,
Android 7.1/API 25 or newer. Original signing identity retained; source excludes private
keys/local configuration and retains licences.
