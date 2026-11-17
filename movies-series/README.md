# ShadowFoxTV Movies & Series 0.3.17

[Signed APK](ShadowFoxTV-Movies-Series-0.3.17.apk) · [Complete source](ShadowFoxTV-Movies-Series-0.3.17-source.zip) · [Updater feed](update.json) · [Verification](verification-0.3.17.json)

TV Settings has a fixed left section menu beside a scrolling content pane. Up/Down browses sections; Right or OK enters its controls. Within the pane, Up/Down follows the enabled controls in order and stops at the bottom. Up from the first control, Left, or remote Back returns to the same section menu. Back again exits Settings. Each section remembers its last focused control and scroll position. Entire focused rows are brought into view, with stable focus size. Busy/disabled actions return focus to an available control or the section menu.

Account editors still require OK. Cancelling returns focus to the original row; changing sections does not save account drafts. Phone Settings retains top section tabs and direct touch editing. Account, Appearance, Playback, Library and Updates remain; Profiles/About are absent. Both Cinema and ShadowFox Exclusive themes are retained.

212 automated tests passed; release lint has no errors. New tests cover initial focus, menu/control paths, bottom clamping, complete row visibility, section focus/scroll restoration, Back, disabled actions, editor cancellation, theme changes and smaller TVs. Both TV themes were rendered locally. Exact signed APK was installed in place and hash-verified on Tanix. Remote-only Account/editor cancellation, Appearance, long Playback navigation, Library and Updates were checked. No account text was entered or saved; no provider stream was started. No physical phone was used. Earlier Tanix 4K/heat issue remains unresolved.

Saved logins, watch progress, continuous browsing, Adult shortcuts, touch support, phone rotation, TV landscape, player/DTS audio and updater are retained. Provider content still depends on the supplied categories. Account storage, SettingsViewModel, database, queries/paging, player, native audio and orientation are byte-identical to 0.3.16. Updater flow is unchanged after normalizing its injected Settings button renderer.

Package `ca.shadowfoxtv.movieseries`, version code 29, Android 7.1/API 25 or newer. Install over the existing app to keep your data. Signed with the original compatible certificate. This feed is separate from Platinum Player.

Complete source includes Inter/OFL fonts, AndroidX Media3/FFmpeg source, four-ABI audio libraries and licenses/provenance. Private signing keys and local configuration are excluded. Original attribution retained; AndroidX Media3 is Apache 2.0 and FFmpeg 6.1.6 LGPL 2.1 or later.
