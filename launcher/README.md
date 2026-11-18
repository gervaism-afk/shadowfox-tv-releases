# ShadowFoxTV Launcher Pro 1.7.2

Version code 28 · package `com.shadowfox.tvlauncher.review`.

Removes the launcher's rounded background panels around individual app icons. App tile boxes default Off, so unfocused apps have no tile fill or border. The selected app uses a short blue-and-amber underline and the existing slight enlargement. Android's default rectangular focus highlight is disabled for app tiles on supported versions.

Native app icon artwork, custom icons and icon-pack images are unchanged. Any shape or background that is part of an app's actual artwork stays intact. This change affects the surrounding launcher panels only, as requested.

Open Settings → Home screen → Transparency → App tile boxes to restore the previous panels. When enabled, they follow the existing App box transparency percentage. Banner and dock transparency remain independent; switching Home transparency Off does not restore individual boxes when App tile boxes is Off. The tile-box choice persists across restarts. Restore appearance defaults returns App tile boxes to Off.

Existing wallpaper, fonts, icon choices, labels, app order, groups and transparency percentages retain their preference keys. ShadowFox Exclusive Wallpapers is unchanged. No additional Android permissions are requested. Normal delivery is through the in-app updater; APK and source files are backups. Package and signing identity are unchanged.

## Build on Windows

Requires Python 3, a Java JDK, Android SDK platform 35 and build-tools 35.0.0. Set `JAVA_HOME` and `ANDROID_HOME` if needed. Set `SHADOWFOX_SIGNING_DIR` to a private directory containing the existing `shadowfox-home.p12` and `password.txt`, then run `python build_launcher_review.py`.

Output: `shadowfox-branding/launcher-review/ShadowFoxTV-Launcher-Pro-1.7.2.apk`. The source archive excludes signing material, device preferences, build outputs and test screenshots. Verification uses a disposable Android TV emulator; no physical TV box was tested.
