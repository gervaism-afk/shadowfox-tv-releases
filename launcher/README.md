# ShadowFoxTV Launcher Pro 1.6.1

Version code 24 · package `com.shadowfox.tvlauncher.review`.

This update makes the 1.6.0 glass design more transparent. With a wallpaper selected, the Home header uses approximately 39% opacity and the app dock 37%. The lower-screen shading is also lighter so more artwork remains visible. Focused controls retain a stronger tint and the existing blue-to-amber border for readability.

Settings now renders its translucent surfaces above your wallpaper, with lighter category, heading and option surfaces. The wallpaper is shown without the Home header or app labels behind the settings text. Option panels use less background dimming, and app selectors and icon browsing share the more transparent materials. Plain Home colour themes and the user's individual app-tile background choice retain their existing behaviour.

The original stock wallpaper, custom wallpaper, saved fonts, app names, groups, ordering, icons and Home layout are retained. The small Home preview stays local to the device. The existing in-app update feed and package/signature checks are unchanged.

## Install and build

Normal delivery is through the launcher's in-app updater. APK and source files are backup copies. Update the existing app without uninstalling or clearing data.

To build on Windows, use Python 3, a Java JDK, Android SDK platform 35 and build-tools 35.0.0. Set `JAVA_HOME` and `ANDROID_HOME` if needed. Set `SHADOWFOX_SIGNING_DIR` to a private directory containing the existing `shadowfox-home.p12` and `password.txt`, then run `python build_launcher_review.py`.

The signed output is `shadowfox-branding/launcher-review/ShadowFoxTV-Launcher-Pro-1.6.1.apk`. Private signing material and copied device data are excluded from this source archive.

Visual and navigation checks use an isolated Android TV emulator. The physical TV box has not been tested for this release. See the separate release verification report for completed checks and file hashes.

