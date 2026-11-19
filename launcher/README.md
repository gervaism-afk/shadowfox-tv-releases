# ShadowFoxTV Launcher Pro 1.9.1

Version code 35 · package `com.shadowfox.tvlauncher.review`.

Reworks the Home rows with compact category names beside the apps and counts immediately below the names. The narrower label column brings each group closer to its icons and reduces horizontal gaps compared with 1.9.0. Rows remain fully free-floating without panels, outlines, shadows, dividers or badges. Saved apps-across, icon sizes, artwork and labels are retained.

Keeps the 1.9.0 compact banner, browsing contrast, focus motion and shared menu typography. No Settings or wallpaper-selector changes are included. Category data, app assignments, wallpaper and saved preferences are retained. Up-to-Home navigation and the Fire TV update/dialog compatibility fixes remain in place.

## Build on Windows

Requires Python 3, a Java JDK, Android SDK platform 35 and build-tools 35.0.0. Set `JAVA_HOME` and `ANDROID_HOME` if needed. Set `SHADOWFOX_SIGNING_DIR` to the private directory containing the existing `shadowfox-home.p12` and `password.txt`, then run `python build_launcher_review.py`.

The source archive excludes signing material, device data, build outputs and test captures.
