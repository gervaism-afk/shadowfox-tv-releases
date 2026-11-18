# ShadowFoxTV Launcher Pro 1.7.0

Version code 26 · package `com.shadowfox.tvlauncher.review`.

Adds **ShadowFox Exclusive Wallpapers**, an offline wallpaper selector with a large preview, thumbnail browsing, a current-wallpaper marker and an explicit Apply wallpaper button. Find it under Settings → Wallpaper → ShadowFox Exclusive Wallpapers. Moving focus previews artwork; OK moves to Apply; Apply saves the choice and returns Home. Back cancels without changing the wallpaper.

The owner-selected collection contains Studio (the earlier blue-and-amber design), Obsidian Silk, Forged Titanium, Glacial Prism and Liquid Copper. Other generated concepts are excluded from the app. Each wallpaper retains the ShadowFox TV shield logo. These five are native opaque 1672 × 941 PNGs; the separate Original artwork remains 3840 × 2160. The selector fits the whole image in its preview; Home scales and crops to the display as before.

Existing wallpaper, dimming, fonts, app labels, groups, app order, icon choices and Home settings retain their existing preference keys. Studio remains the default for a new install. Original artwork, custom images and the plain Theme background remain available. Browsing the collection does not save a preference until Apply is pressed.

Normal delivery is through the in-app updater; the signed APK and source archive are backups. The package and signing identity are unchanged. Emulator verification is recorded separately; this release has not been tested on a physical TV box.

## Build on Windows

Requires Python 3, a Java JDK, Android SDK platform 35 and build-tools 35.0.0. Set `JAVA_HOME` and `ANDROID_HOME` if needed. Set `SHADOWFOX_SIGNING_DIR` to a private directory containing the existing `shadowfox-home.p12` and `password.txt`. Run `python build_launcher_review.py`.

The output is `shadowfox-branding/launcher-review/ShadowFoxTV-Launcher-Pro-1.7.0.apk`. The source archive excludes signing material, device preferences, generated build files and test screenshots.

Wallpaper art was created using the built-in imagegen tool, with the approved Studio wallpaper as the logo reference. Standalone PNGs and generation prompts are supplied separately.
