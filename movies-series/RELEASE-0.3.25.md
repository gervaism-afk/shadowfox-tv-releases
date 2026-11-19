# ShadowFoxTV Movies & Series 0.3.25

[Signed APK](ShadowFoxTV-Movies-Series-0.3.25.apk) · [Complete source](ShadowFoxTV-Movies-Series-0.3.25-source.zip) · [Updater feed](update.json) · [Verification](verification-0.3.25.json)

Opening an existing category filter on TV now places the cursor at the end of the text. The shared TV editor retains text and selection together, so keyboard updates preserve a deliberately moved cursor. Done continues to apply the edited text, and Cancel keeps the existing value. Other TV account fields share this correction; phone direct editing is unchanged.

The issue was reproduced on Tanix: its native keyboard opened the 19-character filter at selection0. The corrected signed APK was installed in place and hash-verified; the real keyboard opened at selection19 on both initial opening and Cancel/reopen. The filter and entire saved-preferences fingerprint were unchanged. The editor was left open for the user; no real filter/account edit was committed or provider playback started.

260 tests passed with zero failures; release lint has zero errors. New regression checks cover appending at the initial end position and middle insertion after manually moving the caret. Existing editor cancellation, password masking, keyboard-safe controls, phone touch and remote navigation checks passed.

Only the version, shared editor and its regression test file differ from0.3.24. Original artwork, the complete0.3.24 polish, account persistence, Adult filtering, database/player/native audio, orientation, updater/security backend and all resources are unchanged. Fire TV was not directly updated in this pass; it can obtain this release through the normal updater. No provider playback was tested; earlier Tanix4K/heat issue remains unresolved.

Package `ca.shadowfoxtv.movieseries`, version code37, Android7.1/API25 or newer. Signed with the original compatible certificate. Install over the existing app to retain data. Complete source retains attribution, Inter/OFL fonts, Media3/FFmpeg sources, native four-ABI audio and licences. Private signing keys and local configuration are excluded.
