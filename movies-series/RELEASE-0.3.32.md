# ShadowFoxTV Movies & Series 0.3.32

[Signed APK](ShadowFoxTV-Movies-Series-0.3.32.apk) · [Source](ShadowFoxTV-Movies-Series-0.3.32-source.zip) · [Updater feed](update.json) · [Verification](verification-0.3.32.json)

Settings now includes About after Updates, with a matching outlined information icon.
It shows the original logo, ShadowFox TV / Movies & Series, a short app description,
and the actual current version and build number. The requested credit is displayed as:

App Created and Developed  
Mandy Gervais  
Copyright 2026, ShadowFox TV

Identity, version and credits are three read-only information blocks. Remote Up/Down
can scroll each block fully into view, Left returns to About, and the final row stops.
Back remains reachable below the six menu sections. Phone layouts scroll normally and
wrap the credit at larger text sizes. Profiles remain absent from Settings.

281 tests passed with zero failures; release lint has zero errors. New
checks cover the last menu section, remote information order/scroll bounds/stop,
footer Back reachability, exact credit and dynamic version, and a narrow phone at
1.3 text scale. TV and phone layouts were visually reviewed. Existing navigation,
saved-account, Adult filtering, orientation, player and updater checks passed.

Installed in place over 0.3.31 on the user's free Fire TV, with the original compatible
signer. The installed APK hash matches the download. Native checks verified Home
startup focus, About access, actual 0.3.32/build44, exact creator/copyright text,
read-only information scrolling/stop, footer Back and remembered credit focus. About
was left open for review. No app data was cleared and configured Home opened. No real
preference, manual refresh or provider-playback action was activated. Audio/system/
display/server/key settings and other devices were untouched; private account files
were not read. Provider playback/audio/connectivity were not tested.

Only version and SettingsScreen change in production, with new AboutSettings; the two
existing navigation test fixtures are updated and AboutSettingsTest is added. All
resources including the exact original logo, account storage/schema, database, Home
focus repair, player, updater backend and orientation files are byte-identical to 0.3.31.
Package `ca.shadowfoxtv.movieseries`, code 44, Android 7.1/API 25 or newer. Original signing
identity retained; source excludes private keys/local configuration and retains licences.
