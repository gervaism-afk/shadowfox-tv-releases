# ShadowFoxTV Launcher Pro 1.7.4

Version code 30 · package `com.shadowfox.tvlauncher.review`.

Fixes Fire TV update compatibility and the narrow, clipped settings window seen on the tested Amazon AFTHA004 / Fire OS API 28.

The updater requests both modern and legacy signing-certificate metadata on Android 9 and newer. Fire OS returned no archive certificate for the modern flag alone, but returned the correct certificate when both flags were requested. SHA-256, package identity, expected/newer version and exact nonempty signer-set checks remain enforced. HTTPS validation stays enabled; the signing key and permissions are unchanged.

Custom settings, option panels, wallpaper selector and icon browser now own their dialog content frames directly. This avoids Fire OS's fixed-size native alert-content container while retaining the app's existing fullscreen and side-panel sizing, remote navigation and Back behavior. Native confirmation and text-entry dialogs are unchanged.

Affected older installations need a one-time signed repair bridge because their updater cannot validate the fix itself. That repair uses an in-place update and retains app data. The final release is then downloaded and installed through the normal launcher updater. Wallpaper choices, app labels, groups, icons and transparency settings keep their existing preference keys.

## Build on Windows

Requires Python 3, a Java JDK, Android SDK platform 35 and build-tools 35.0.0. Set `JAVA_HOME` and `ANDROID_HOME` if needed. Set `SHADOWFOX_SIGNING_DIR` to a private directory containing the existing `shadowfox-home.p12` and `password.txt`, then run `python build_launcher_review.py`.

Output: `shadowfox-branding/launcher-review/ShadowFoxTV-Launcher-Pro-1.7.4.apk`. APK and source files are backups; normal delivery uses the in-app update feed. The source archive excludes repair bridge APKs, diagnostics, signing material, device preferences, build outputs and test captures. Device and delivery checks are recorded separately.
