# ShadowFoxTV Launcher Pro 1.8.0

Version code 32 · package `com.shadowfox.tvlauncher.review`.

Redesigns Home categories as distinct glass shelves. Rounded translucent panels, a lit upper rim, a soft underside shadow and a restrained reflective gradient give each category depth while keeping the wallpaper visible. Category names and compact counts sit beside the app rails with a quiet divider. The active category gains a blue-and-amber accent and its count shows the focused app's position, such as 8 / 10. Individual app icons retain their artwork and box-free underline focus treatment.

The layout reserves space for the category label and adapts the app rail to the remaining width. Automatic apps-across can therefore fit a different count on narrower displays; saved explicit density, icon-size, font, label and transparency preferences are retained. Shelf surface opacity follows the existing App box transparency control; a fine structural rim remains visible at high transparency, including Clear. No new preference or category migration is needed.

Up still traverses category rows and restores the main Home view when focus reaches the header. The first shelf's Home dock measurement now uses the complete category row. Category names, app assignments, ordering, custom icons, wallpaper and groups keep their existing data. Empty categories offer Choose apps and remain usable with the remote.

The Fire TV certificate and custom-dialog compatibility fixes are retained. Package, signing identity, permissions and normal in-app update delivery are unchanged. APK and source files are backups.

## Build on Windows

Requires Python 3, a Java JDK, Android SDK platform 35 and build-tools 35.0.0. Set `JAVA_HOME` and `ANDROID_HOME` if needed. Set `SHADOWFOX_SIGNING_DIR` to a private directory containing the existing `shadowfox-home.p12` and `password.txt`, then run `python build_launcher_review.py`.

Output: `shadowfox-branding/launcher-review/ShadowFoxTV-Launcher-Pro-1.8.0.apk`. The source archive excludes signing material, device data, build outputs and test captures.
