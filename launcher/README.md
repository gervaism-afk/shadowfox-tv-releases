# ShadowFoxTV Launcher Pro 2.3.1

Version code 40 · package `com.shadowfox.tvlauncher.review`.

Home now contains only app shortcuts: Your apps and Recently opened. Shared preview channels, Continue watching programs, movie/series recommendations and their poster loaders are removed for every provider, including Apple TV and Spotify. The TV provider reader, content observer, READ_TV_LISTINGS permission and obsolete recommendation controls are removed. Previously granted TV-listing access cannot bring those rows back.

The top-left Quick launch block is removed, including the selected app title, Open button, and group caption. The corresponding Set Quick launch app-menu option is also removed. D-pad Down from Home goes directly to Your apps; Up returns to the tabs.

The current branded header, www.shadowfoxtv.ca, custom static wallpaper, icon artwork, transparency settings and app assignments remain in use. Your apps remains near the bottom of the first screen; Recently opened is reached by scrolling down and uses matching app icons. The Apps page retains saved category filters and the full app library. Existing app options remain available with MENU or a long press. Wallpapers remain available in Settings.

The update signing identity, download/certificate verification, Fire TV dialog compatibility and wallpaper selector implementations are unchanged. Existing app data is retained; no new permissions are requested.

## Build on Windows

Requires Python 3, a Java JDK, Android SDK platform 35 and build-tools 35.0.0. Set JAVA_HOME and ANDROID_HOME if needed. Set SHADOWFOX_SIGNING_DIR to the private directory containing the existing shadowfox-home.p12 and password.txt, then run python build_launcher_review.py.

The source archive excludes signing material, device data, test fixtures, build outputs and captures.
