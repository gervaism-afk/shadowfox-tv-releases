# ShadowFoxTV Launcher Pro 1.8.1

Version code 33 · package `com.shadowfox.tvlauncher.review`.

Category labels, app counts and icons now float directly over the wallpaper. Removes the glass shelf surfaces, outlines, shadows, dividers, accent bars and count badges introduced in 1.8.0. The active category retains a text colour cue, and selected apps retain their existing underline focus treatment. App artwork and the saved individual tile box preference are unchanged.

Keeps category spacing, horizontal scrolling, app positions and Up-to-Home navigation. Category assignments, custom icons, wallpaper and saved appearance settings are retained. Banner transparency and optional individual app tile transparency remain adjustable; category rows have no background at any opacity setting.

Fire TV certificate and dialog compatibility fixes remain in place. Package and signing identity are unchanged, supporting the normal in-app update flow.

## Build on Windows

Requires Python 3, a Java JDK, Android SDK platform 35 and build-tools 35.0.0. Set `JAVA_HOME` and `ANDROID_HOME` if needed. Set `SHADOWFOX_SIGNING_DIR` to a private directory containing the existing `shadowfox-home.p12` and `password.txt`, then run `python build_launcher_review.py`.

Output: `shadowfox-branding/launcher-review/ShadowFoxTV-Launcher-Pro-1.8.1.apk`. The source archive excludes signing material, device data, build outputs and test captures.
