# ShadowFoxTV Launcher Pro 1.6.2

Version code 25 · package `com.shadowfox.tvlauncher.review`.

Adds the Studio wallpaper: graphite and smoked-glass textures, blue and amber edge lighting, and the ShadowFox TV shield logo. The logo sits above the app dock and the top and lower areas stay quiet for the transparent interface. The selected native wallpaper asset is an opaque 1672 × 941 PNG; Android scales/crops it to the display. The separate original wallpaper remains 3840 × 2160.

Choose Settings → Wallpaper → Studio wallpaper. Studio is the default when no wallpaper mode has been saved. A previously saved Original artwork, Theme background or custom image choice is retained. Original artwork remains available as a separate option.

Existing fonts, labels, groups, app order, artwork, icon packs, dimming and other Home settings retain their existing preference keys. The built-in updater and signing identity are unchanged. Normal delivery is through the in-app updater; APK and source files are backups.

## Build on Windows

Requires Python 3, a Java JDK, Android SDK platform 35 and build-tools 35.0.0. Set `JAVA_HOME` and `ANDROID_HOME` if needed. Set `SHADOWFOX_SIGNING_DIR` to a private directory containing the existing `shadowfox-home.p12` and `password.txt`. Run `python build_launcher_review.py`.

The signed output is `shadowfox-branding/launcher-review/ShadowFoxTV-Launcher-Pro-1.6.2.apk`. The archive excludes signing material, copied device preferences and test screenshots.

The wallpaper was created with the built-in imagegen tool using the existing stock wallpaper's logo as the image-edit reference. The standalone wallpaper and full generation prompts are saved separately as user deliverables. Emulator checks are recorded in the separate release verification report; this release has not been tested on the physical TV box.

