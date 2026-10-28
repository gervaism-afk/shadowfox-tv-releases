# ShadowFoxTV Movies & Series 0.3.3

Version code 15. Signed with the same certificate as 0.3.2, allowing an in-place update that preserves saved accounts and progress.

Phone browsing supports portrait and landscape while respecting the user's rotation setting. Navigation stays on the current screen during rotation. Narrow library, settings and detail layouts adapt to phones. Android TV browsing and playback retain landscape. Apple TV inspired Home, touch/remote input and the existing updater remain in place.

Validation: 135 unit/Compose tests passed; release lint has zero errors. Installed over 0.3.2 on a phone emulator and verified saved account/catalogue retention, portrait home/library/details, touch navigation and rotation. Android TV emulator landscape and D-pad navigation passed. Real provider playback and physical streamer testing were not completed; the streamer remained unauthorized over ADB.

Install as an update. Do not uninstall or clear app storage.
