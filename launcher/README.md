# ShadowFoxTV Launcher Pro 1.6.0

Version code 23 · package `com.shadowfox.tvlauncher.review`.

Home now uses a translucent graphite header and app dock, a framed brand emblem, shelf accents and app counts. The focused app lifts slightly inside a blue-to-amber outline. Header controls use matching shaped surfaces. The original stock 4K wallpaper and custom wallpaper choices remain available.

Settings, option pickers and app checklists share layered surfaces, blue highlights and warm accents. The settings header includes a small preview of the actual Home screen, including its saved wallpaper, font, app layout and artwork. This preview is generated locally when settings opens and released when the page closes; it is never uploaded. Setting rows use control symbols and separate value badges.

No preference migration is required. Existing themes, fonts, labels, groups, app order, artwork, icon packs, wallpaper and layout choices retain their existing keys. Both light and dark Home themes are supported. The in-app updater retains its existing HTTPS feed, checksum verification, package/version checks and signing-certificate verification.

## Delivery

Normal delivery is through the launcher's built-in update feed. APK and source copies are backups. Install over the existing launcher without uninstalling or clearing its data.

## Build on Windows

Requires Python 3, a Java JDK, Android SDK platform 35 and build-tools 35.0.0. Set `JAVA_HOME` and `ANDROID_HOME` if needed. Set `SHADOWFOX_SIGNING_DIR` to the private directory containing the existing `shadowfox-home.p12` and `password.txt`. Run `python build_launcher_review.py`. Signing material and copied device data are excluded from this archive.

The output is `shadowfox-branding/launcher-review/ShadowFoxTV-Launcher-Pro-1.6.0.apk`. The release retains the ShadowFox TV Home signing identity so it can update existing installations.

## Verification scope

Visual and remote-navigation checks use an isolated, disposable Android TV API 36 emulator. Screenshots show temporary test preferences. Physical TV hardware has not been tested for this release. See the separate release verification report for completed checks and the APK digest.

