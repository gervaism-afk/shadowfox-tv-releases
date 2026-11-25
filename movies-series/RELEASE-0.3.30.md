# ShadowFoxTV Movies & Series 0.3.30

[Signed APK](ShadowFoxTV-Movies-Series-0.3.30.apk) · [Source](ShadowFoxTV-Movies-Series-0.3.30-source.zip) · [Updater feed](update.json) · [Verification](verification-0.3.30.json)

Home's Play, Details and New picks actions now use consistent vector icons. Movies,
Series and My List shelves have View all actions into their existing complete collections.
These links do not start playback. The first Continue Watching card still fits on the
compact TV layout. The startup Home focus and return-to-poster behavior are retained.

Movie and series details offer a visible Back button for both touch and remote use.
Up from the action row reaches Back; Down scrolls the header into view before returning
to the primary action, including after a long page has disposed that header. Play retains
initial focus without stealing it when metadata arrives. Primary actions share the
Home treatment and minimum48dp controls. A missing/loading movie no longer leaves a
blank canvas: its themed status view includes an exit.

Search identifies movies versus series and describes matching results, saved titles
or the selected collection accurately. Empty results suggest changing the query;
missing Adult categories still explain the actual provider limitation. Library text
uses the selected theme's palette; long query subtitles are bounded to one line.
Continuous paging and remembered grid position remain.

273 tests passed, zero failures; release lint has zero errors. Checks cover
remote and touch collection links without playback, detail Back/Play navigation,
phone loading/unavailable exit, contextual counts/empty states, existing TV/phone Home
bounds, touch targets, Settings editors, saved-account behavior, Adult filtering,
orientation and updater rules. Rendered previews use synthetic fixture artwork.

Physical installation is pending availability of the intended Fire TV. No device
commands were sent in this pass. Physical Fire TV behavior, real provider connectivity/playback and audio
have not been tested for this release. No performance improvement is claimed.

The original logo and all resources are byte-identical to0.3.29. Account storage/schema,
database, Settings, native player code, updater backend and orientation are unchanged.
Only the shared control component changes player button shape/minimum height. Package
`ca.shadowfoxtv.movieseries`, code42, original compatible signing certificate, minAndroid
7.1/API25. Source excludes private keys/local configuration and retains licences.
