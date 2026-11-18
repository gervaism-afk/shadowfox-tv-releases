# ShadowFoxTV Launcher Pro 1.7.3

Version code 29 · package `com.shadowfox.tvlauncher.review`.

Fixes the Fire TV update error **The update has no signing certificate**. On the tested Amazon AFTHA004 running Fire OS/API 28, PackageManager returns the installed launcher's certificate with GET_SIGNING_CERTIFICATES, but omits certificate data for an APK archive when that flag is requested alone. Requesting both GET_SIGNING_CERTIFICATES and GET_SIGNATURES returns the verified archive certificate. The updater now requests both on Android 9 and newer, with a legacy certificate-field fallback only when modern metadata is absent.

APK SHA-256, package name, exact expected version, newer-version requirement and nonempty signer-set equality are still enforced. A mismatching modern certificate does not fall back to a different certificate. HTTPS certificate validation remains enabled. The signing key and Android permissions are unchanged.

Older affected installations cannot download their own fix through the broken verifier. The affected Fire TV received a one-time signed repair bridge as an in-place update; its app data was retained. The final 1.7.3 release is delivered through the normal updater. Other devices receive the normal in-app release.

Wallpaper choices, transparency controls, box-free app tiles, labels, icon choices and app groups are unchanged from 1.7.2. APK and source files are backups; normal distribution is through the existing HTTPS update feed.

## Build on Windows

Requires Python 3, a Java JDK, Android SDK platform 35 and build-tools 35.0.0. Set `JAVA_HOME` and `ANDROID_HOME` if needed. Set `SHADOWFOX_SIGNING_DIR` to a private directory containing the existing `shadowfox-home.p12` and `password.txt`, then run `python build_launcher_review.py`.

Output: `shadowfox-branding/launcher-review/ShadowFoxTV-Launcher-Pro-1.7.3.apk`. The source archive excludes the private repair bridge, diagnostic app, signing material, device preferences, build outputs and test captures. Physical-device and delivery checks are recorded separately.
