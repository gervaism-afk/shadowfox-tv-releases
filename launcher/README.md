# ShadowFoxTV Launcher Pro 1.7.1

Version code 27 · package `com.shadowfox.tvlauncher.review`.

Home now has adjustable transparency for its banner, banner controls, app dock and app boxes. Open Settings → Home screen → Transparency. Home transparency switches the backgrounds between transparent and solid. Banner transparency and App box transparency have independent levels: 0%, 25%, 50%, 75%, 90% and 100%. Higher percentages reveal more wallpaper; 0% is solid and 100% removes the material fill. Text, app artwork and the blue-and-amber focus outline stay visible.

Transparency defaults On at 75% for both groups. Turning it Off retains both chosen percentages and shows solid surfaces. While Off, intensity rows show their saved values; changing them updates the saved intensity without enabling transparency. Turning On restores those saved levels. Restore appearance defaults resets all three transparency settings too.

These controls replace the previous Tile background choice, so app boxes and the dock follow one intensity without conflicting settings. Wallpaper dimming remains independent. The five ShadowFox Exclusive wallpapers, original artwork, custom images and theme backgrounds remain available. Existing wallpaper, fonts, app labels, icons, groups and app order keep their existing preferences. This release does not request any additional Android permissions.

Normal delivery is through the in-app updater. Signed APK and source files are backups. The package and signing identity are unchanged. Verification was performed on a disposable Android TV emulator, not a physical TV box.

## Build on Windows

Requires Python 3, a Java JDK, Android SDK platform 35 and build-tools 35.0.0. Set `JAVA_HOME` and `ANDROID_HOME` if needed. Set `SHADOWFOX_SIGNING_DIR` to a private directory containing the existing `shadowfox-home.p12` and `password.txt`, then run `python build_launcher_review.py`.

The output is `shadowfox-branding/launcher-review/ShadowFoxTV-Launcher-Pro-1.7.1.apk`. The source archive excludes signing material, device preferences, build outputs and test screenshots.
