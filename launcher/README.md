# ShadowFoxTV Launcher Pro 1.4.10

Press Home to return to your app row, including from launcher settings or an unsaved label/category editor. The launcher uses a single Home activity and closes its editing panels on Home without saving unsaved text.

Settings → Wallpaper → Choose an image and Hold OK on an app → Change icon → Choose an image prefer Android's folder/storage file picker. Devices without a supported file picker fall back to an image/gallery picker. Storage providers determine available local, USB and cloud locations. The launcher copies the selected image into its own storage; it does not need permanent access to the original file. Android's [Storage Access Framework documentation](https://developer.android.com/training/data-storage/shared/documents-files) describes this picker mechanism.

Image decoding, resizing and saving run in the background. You can return Home while an image saves. The supplied 3840×2160 stock wallpaper is unchanged. Large custom wallpaper images retain up to 3840 pixels on their longest edge; custom app icons are prepared as square images up to 512 pixels. Invalid image files leave the previous image intact.

Settings → Navigation sounds controls Android's standard navigation effects, without changing playback volume. Apps playing their own custom sounds may require their own setting. Some TV firmware lacks Android's Modify system settings permission page; the tested H96 needed a one-time grant through ADB. Its On/Off readback and unchanged playback volumes were verified.

Install this APK as an update to the existing ShadowFoxTV Launcher Pro, without uninstalling or clearing data, to keep your apps, categories, order, labels, icons, wallpaper and appearance. Its internal package remains com.shadowfox.tvlauncher.review and it retains the existing signing identity. Select ShadowFoxTV Launcher Pro → Always if Android asks you to choose Home.

Settings → Launcher updates → Check for updates uses the existing GitHub feed. The launcher verifies the downloaded APK's SHA-256, package, version and signing certificate before opening Android's installer. It requires the device's installation permission for the launcher.

H96 checks and update-flow results are in launcher-pro-1.4.10-verification.json. This release was not installed on Fire TV or the unavailable Tanix. The H96 Bluetooth repair remains a separate installed helper and is unaffected by this launcher update.

APK: https://raw.githubusercontent.com/gervaism-afk/shadowfox-tv-releases/main/launcher/ShadowFoxTV-Launcher-Pro-1.4.10.apk

The source archive excludes signing keys, device preferences and test snapshots. Rebuilding requires your signing key, Android SDK 35/build-tools 35.0.0, Java and Python, with local paths adjusted in build_launcher_review.py.
