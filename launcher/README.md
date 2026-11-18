# ShadowFoxTV Launcher Pro 1.7.5

Version code 31 · package `com.shadowfox.tvlauncher.review`.

Fixes category shelves remaining scrolled over the wallpaper after Up returns focus to the Home header. Header controls are outside the category ScrollView, so Android was moving focus without restoring its scroll position. Focusing a Home header control now smoothly scrolls the shelves back to their Home position.

Up still moves back through the category rows. When focus reaches the header, Home returns to its normal overview and first-shelf position. Returning from Settings to the header also restores that view. Existing category names, app assignments, order, icon artwork, wallpaper and layout preferences are unchanged.

The fix was reproduced and checked on the user's Tanix TX68 with multiple existing categories. Other-device certificate and Fire TV dialog fixes from 1.7.4 are retained. Package, signing identity, Android permissions and update feed are unchanged. Normal delivery uses the in-app updater; APK and source files are backups.

## Build on Windows

Requires Python 3, a Java JDK, Android SDK platform 35 and build-tools 35.0.0. Set `JAVA_HOME` and `ANDROID_HOME` if needed. Set `SHADOWFOX_SIGNING_DIR` to a private directory containing the existing `shadowfox-home.p12` and `password.txt`, then run `python build_launcher_review.py`.

Output: `shadowfox-branding/launcher-review/ShadowFoxTV-Launcher-Pro-1.7.5.apk`. The source archive excludes signing material, device data, build outputs and test captures.
