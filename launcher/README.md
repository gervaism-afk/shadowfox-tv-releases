# ShadowFoxTV Launcher Pro 1.5.0

Version code: 22. Package: `com.shadowfox.tvlauncher.review`.

This release replaces the settings menu with a full-screen TV workspace. A category rail leads to Appearance, Home screen, Wallpaper, Apps & groups, Sound & device, and Updates. Rows separate the setting name, explanation, and current value. Option pickers and app checklists share a dark palette, rounded controls, and clear focus borders.

The existing preference keys, categories, app order, labels, icons, wallpaper, and update verification remain in use. Settings typography stays readable independently of the Home font or colour theme. Android device settings open above the dashboard, so Back returns to the originating control. The Home button closes launcher dialogs and discards unsaved checklist changes.

## Install

Install the signed APK as an update over the existing launcher. Do not uninstall it or clear its data. The release uses the existing ShadowFox TV Home signing certificate. If Android asks for a Home app, choose ShadowFoxTV Launcher Pro.

## Build on Windows

Requires Python 3, a Java JDK, Android SDK platform 35, and Android build-tools 35.0.0. No Gradle dependency download is required.

Set `JAVA_HOME` to the JDK directory and `ANDROID_HOME` to the Android SDK directory if they differ from the script's Android Studio defaults. Set `SHADOWFOX_SIGNING_DIR` to a private directory containing the existing `shadowfox-home.p12` and its `password.txt`. Signing material is intentionally excluded from this source archive.

Run `python build_launcher_review.py` from this directory. The signed output is `shadowfox-branding/launcher-review/ShadowFoxTV-Launcher-Pro-1.5.0.apk`. The resource cache is regenerated when resource content changes.

## Verification scope

The settings flow was exercised in an Android TV API 36 emulator at 1920 × 1080 and 1280 × 720, including an in-place upgrade from 1.4.13. Verification covers focus navigation, saved font retention, changing options, scrolling, clock and wallpaper controls, app checklist Save/Cancel, and Back from Android device settings. The final release was signature-verified against 1.4.13. Physical-device checks and publishing to the live update feed are separate from this build.

