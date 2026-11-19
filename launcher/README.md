# ShadowFoxTV Launcher Pro 2.1.0

Version code 37 · package `com.shadowfox.tvlauncher.review`.

Home now follows the owner's Google TV reference: pill-shaped Home and Apps navigation, wide cards, circular app icons, wallpaper and settings shortcuts, and a category-filtered Apps library. The existing ShadowFox header implementation is retained unchanged. The owner's saved app groups, order, labels, hidden apps, custom artwork, icon-pack selection, typography and transparency preferences remain in use.

The background is a static image. There is no video player, autoplay, background preview video or Google account integration. ShadowFox keeps its own identity.

## Real recommendations and offline shortcuts

Home reads Android TV PreviewProgram channels and Watch Next CONTINUE records when the device and installed apps expose them. Choose Settings → Apps & groups → App recommendations to allow Android's read-only TV-listings permission. Channels/programs marked not browsable are excluded. Hidden or uninstalled source apps are excluded. Without accessible recommendation rows, Featured apps uses real installed-app banners and shortcuts. Recently opened records successful launches through this launcher; it is separate from Continue watching.

Program cards launch the publishing app's deep link. The target is restricted to its installed owner package, with app launch as the fallback when a link is invalid. Static posters load in bounded background workers and a bounded memory cache. Missing providers, denied permission, missing poster images and offline use retain working app shortcuts. Shared TV data is read-only; no privileged system permissions or TV-provider write permission is requested.

Android's data model: [PreviewPrograms](https://developer.android.com/reference/android/media/tv/TvContract.PreviewPrograms), [WatchNextPrograms](https://developer.android.com/reference/android/media/tv/TvContract.WatchNextPrograms), and [TV provider permission handling](https://android.googlesource.com/platform/packages/providers/TvProvider/+/master/src/com/android/providers/tv/TvProvider.java).

## Wallpaper and controls

Midnight Flow is a new dark indigo and blue wallpaper with the owner's ShadowFox logo, composed to leave room for navigation and cards. It is the default for new setups; explicit existing wallpaper selections are retained. Cosmic Horizon and the five earlier Exclusive Wallpapers remain selectable. The new wallpaper was applied on the owner's Tanix through the normal selector. Previous custom wallpaper files are retained.

Use Home/Apps tabs with OK; Down enters cards or app rows. Up from the first row returns to navigation, then Up reaches the existing header. Back returns to Home. MENU or holding OK opens app options. Remote reorder uses Left/Right, OK to save and Back to cancel. Empty categories offer Choose apps. All apps / Hidden label settings apply to the Google TV style; Logo dock retains its selected-label option.

App dashboard and Logo dock remain in Settings → Home screen → Home layout. Circular icon surrounds can use the saved app-box background/opacity controls; the header retains its existing transparency controls. App density controls the Apps grid, and icon size controls circular artwork.

The 1.7.3 Fire TV certificate verification fix and 1.7.4 custom-dialog compatibility fix remain unchanged. Update package name and release signing identity are unchanged.

## Build on Windows

Requires Python 3, a Java JDK, Android SDK platform 35 and build-tools 35.0.0. Set `JAVA_HOME` and `ANDROID_HOME` if needed. Set `SHADOWFOX_SIGNING_DIR` to the private directory containing the existing `shadowfox-home.p12` and `password.txt`, then run `python build_launcher_review.py`.

The source archive excludes signing material, device data, test fixtures, build outputs and captures.
