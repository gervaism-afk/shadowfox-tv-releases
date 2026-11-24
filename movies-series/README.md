# ShadowFoxTV Movies & Series 0.3.29

[Signed APK](ShadowFoxTV-Movies-Series-0.3.29.apk) · [Complete source](ShadowFoxTV-Movies-Series-0.3.29-source.zip) · [Updater feed](update.json) · [Verification](verification-0.3.29.json)

All four settings improvements ship together. Appearance offers read-only Home samples in each theme's actual palette, with the exact original artwork. The samples are labelled SAMPLE; they show layout and colours without loading provider content, starting media or adding focus targets. Choosing a theme still requires OK or a tap.

Playback is grouped into Picture, Sound, Subtitles and Trailers. The headings are not remote stops; the six existing controls retain their original settings/callbacks, with an ordered vertical path and remembered return focus. Settings keeps the flat rows and slim marker.

Account shows the actual manual connection-test status, with useful failure guidance and no raw transport URLs. Editing account details invalidates a prior result; an in-flight response cannot verify different credentials. The Library page shows actual refresh progress/error and the existing stored last-successful-refresh time. Loading history, never refreshed, previous success and a newer failure are distinct states. These changes do not trigger a test or refresh automatically and introduce no new stored preference keys.

Phone fields and TV editors use consistent theme colours. Done and Cancel have matching touch targets; Done updates the field draft, while Save on the Account page persists account changes. Caret-at-end, manual cursor movement, cancellation, password masking and focus restoration are retained.

268 tests passed with zero failures; release lint has zero errors. New checks cover credential edits during an in-flight connection test, safe status/error output, refresh loading/error precedence, actual grouped remote navigation and bounds, read-only theme previews and narrow-phone selection. Existing editor, saved-account, Adult, orientation, updater and Home-focus checks passed. TV and phone previews were visually reviewed.

Physical installation and native validation are pending Fire TV debugging authorization. The connection reports unauthorized, so no install, app launch or navigation input was performed in this pass. The signed release is available through the normal verified in-app updater and direct download. No Tanix, startup, system or display changes were made. Provider connectivity/playback was not tested.

Five existing files and two new files differ from 0.3.28: version, AppearanceSettings, SettingsLayout, SettingsScreen, SettingsViewModel; new SettingsStatus and SettingsExperienceTest. Original logo/resources, saved-account storage, player/database, updater backend and orientation are unchanged. Refresh connectivity and provider playback were not tested. Package `ca.shadowfoxtv.movieseries`, version code 41, Android 7.1/API 25 or newer. Source retains attribution, fonts, Media3/FFmpeg and licences; private keys/local configuration are excluded.
