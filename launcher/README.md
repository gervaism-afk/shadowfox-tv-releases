# ShadowFoxTV Launcher Pro 2.5.2

Version code 44 · package `com.shadowfox.tvlauncher.review`.

Recently opened has been removed from Home. Only your saved app categories are shown. Home category app rows are centred when their icons fit in the viewport. App spacing is symmetrical, with no trailing gap after the last icon. Longer rows retain horizontal scrolling and the existing D-pad navigation. Incomplete app-grid rows on the Apps page are centred as well. Category-filter chips and the top Home/Apps navigation retain their previous alignment.

Existing category names, order, app assignments, labels, artwork, transparency, wallpaper selection, automatic ISP weather and all 39 Exclusive Wallpapers are retained. No app-data reset, category migration or additional permissions are required. Signing and update verification are unchanged.

Weather credits remain available in the widget options: MET Norway (CC BY 4.0), GeoJS / MaxMind GeoLite2, and Photon / OpenStreetMap contributors (ODbL).

## Build on Windows

Requires Python 3, a Java JDK, Android SDK platform 35 and build-tools 35.0.0. Set JAVA_HOME and ANDROID_HOME if needed. Set SHADOWFOX_SIGNING_DIR to the private directory containing the existing shadowfox-home.p12 and password.txt, then run python build_launcher_review.py.

The source archive excludes signing material, device preferences, cached locations/weather, test fixtures and build outputs.

