# ShadowFoxTV Movies & Series 0.3.7 (19)

Fixed the remaining Google TV Settings editor overlap: Cancel and Done stay above the keyboard. The editor handles its own keyboard insets, resizes, and scrolls when space is limited.

Settings keeps the fixed header/Back, OK-to-edit TV account rows, remote scrolling to About, and direct phone editing. The cinematic Home UI, fresh picks, portrait browsing, touch controls, saved account, watch progress, player, and updater are retained.

Validation: 147 automated tests passed; release lint has no errors. On Google TV Streamer, 24 Down presses reached About without opening an editor. Three open/cancel cycles were checked with the keyboard visible. No real account values were typed or saved. The APK retains the original signing certificate and installs over the existing app.

Real provider playback was not exercised for this Settings-only change. Exact checksums and validation results accompany the APK and source archive.

Remote OK and Back were also verified on the streamer, including focus returning to the account row.
