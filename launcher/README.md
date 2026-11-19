# ShadowFoxTV Launcher Pro 2.2.0

Version code 38 · package `com.shadowfox.tvlauncher.review`.

Home has a new quick-launch area, simpler navigation and a more compact layout. The existing ShadowFox header and static wallpaper are retained. Selection details use the space that was previously empty: an app's name/category, or a recommendation's title/source. The Open action follows that selection. At Home, Quick launch uses the chosen app, or the first visible app when no choice has been saved.

## Quick launch and Home order

Hold OK or press MENU on an app, then choose Set Quick launch. The selected app is remembered independently of app order, including after a cold start. Hidden or uninstalled choices fall back to the first visible app.

Settings → Home screen → Home content offers Recommendations first and Apps first. Both orders retain Quick launch, app shortcuts and shared recommendation rows. Recommendations first is the default. Continue watching and Recently opened are separate rows and can both appear.

## Artwork and navigation

Poster images retain their proportions instead of being cropped into wide cards. Provider aspect hints set the initial size; decoded image dimensions refine it while preserving the focused item. Captions sit below the artwork, with fuller selection details above. Movie banners stay wide; square covers use square frames. Missing artwork uses its installed app's icon. HTTPS poster redirects are limited and remain HTTPS.

App artwork is fitted from its visible alpha bounds. Transparent wordmarks become easier to read, and detailed app logos retain their artwork. Simple native icon backgrounds can keep a circular mask. Turning app tile boxes Off now removes the launcher-added icon background completely; optional backgrounds still use the saved opacity. Focus rings remain visible independently of opacity. Original icon files and icon-pack preferences are retained.

Home and Back reset horizontal app/content rails to their beginnings. Pressing Home or Back on an already-visible Home page resets its position without rebuilding it. App menus restore the originating control after Cancel, and provider refreshes retain the focused item when it remains available. Category headings show the selected category and its visible app count. Empty categories keep their Choose apps action.

## Recommendations, wallpaper and compatibility

Recommendations are read from installed apps through Android TV's system provider when permitted. Enable Settings → Apps & groups → App recommendations to allow TV-listing access. Without accessible shared rows, Featured apps provides real installed-app shortcuts. Watch Next CONTINUE records supply Continue watching; actual successful launcher app launches supply Recently opened. No catalog or viewing history is fabricated.

Program cards and their contextual Open action restrict deep links to the publishing installed app, with normal app launch as fallback. The TV provider remains read-only. Background images remain static, with no autoplay or background video. [Android's PreviewPrograms reference](https://developer.android.com/reference/android/media/tv/TvContract.PreviewPrograms) documents the poster-aspect metadata used here.

All seven Exclusive Wallpapers remain available, including Midnight Flow and Cosmic Horizon, with existing wallpaper selections retained. App dashboard and Logo dock remain available in Home layout settings. Saved categories, assignments, ordering, labels, hidden apps, artwork, typography and transparency settings are retained.

The existing Fire TV update-signature compatibility fix, release signing identity and custom-dialog compatibility fix remain unchanged.

## Build on Windows

Requires Python 3, a Java JDK, Android SDK platform 35 and build-tools 35.0.0. Set JAVA_HOME and ANDROID_HOME if needed. Set SHADOWFOX_SIGNING_DIR to the private directory containing the existing shadowfox-home.p12 and password.txt, then run python build_launcher_review.py.

The source archive excludes signing material, device data, test fixtures, build outputs and captures.
