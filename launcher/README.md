# ShadowFoxTV Launcher Pro 1.9.0

Version code 34 · package `com.shadowfox.tvlauncher.review`.

Polishes Home, Settings, option panels and the exclusive wallpaper selector. Home keeps its floating app rows and the owner's logo. Category headings sit immediately above their app rails, with compact counts at the trailing edge. Tighter vertical spacing and a 56dp banner give apps a clearer hierarchy. The second category stays outside the collapsed wallpaper showcase.

A lightweight gradient fades in over the wallpaper while browsing expanded categories and fades out on return to Home. This contrast layer does not alter wallpaper files or saved dimming/transparency settings. Theme-only backgrounds skip this layer. App labels gain a restrained readability shadow over wallpaper.

Focused Home icons ease into a small lift and enlargement, retaining the existing blue-and-amber underline and box-free default. Motion cancels the previous transition before starting, so quick remote inputs do not queue animations.

Settings, option panels and the wallpaper selector share typography from the saved font and text-size preferences, a common heading scale and consistent selection surfaces. Settings removes the large preview card and redundant glyph/value boxes. Wallpaper preview and Apply behavior are unchanged.

Category data, app ordering, assignments, custom artwork, chosen wallpaper and existing preferences are retained. Up-to-Home navigation and Fire TV certificate/dialog compatibility fixes remain. The package and release signing identity are unchanged.

## Build on Windows

Requires Python 3, a Java JDK, Android SDK platform 35 and build-tools 35.0.0. Set `JAVA_HOME` and `ANDROID_HOME` if needed. Set `SHADOWFOX_SIGNING_DIR` to the private directory containing the existing `shadowfox-home.p12` and `password.txt`, then run `python build_launcher_review.py`.

The source archive excludes signing material, device data, build outputs and test captures.
