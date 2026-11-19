# ShadowFoxTV Launcher Pro 2.3.0

Version code 39 · package `com.shadowfox.tvlauncher.review`.

## Landing screen

Home and Apps now have matching vector icons and clear focus states. The wallpaper shortcut on the right and the Hold OK for options caption have been removed. App options remain available with MENU or a long press, and wallpapers remain available through Settings.

Your apps sits near the bottom of the first viewport. Its position uses the measured viewport and actual text/icon sizes, including the larger header. Recently opened starts below that viewport and appears when scrolling down. It uses the same app-icon renderer, tile dimensions, labels, opacity and focus treatment as Your apps.

Spotify-owned shared recommendation channels and Watch Next records are filtered. The installed Spotify app and its recent-launch shortcut remain available. Other installed apps can still provide shared programs in the scrolling content below Your apps. No replacement featured-app banner is inserted into the space left by Spotify.

Settings → Home screen → Home content now orders the lower rows: Recommendations first or Recently opened first. Your apps stays on the first screen in both cases. Quick launch, saved categories, app assignments, custom icons and existing app order remain in use.

## Header and text

The header is 70 dp tall, increased from 56 dp, with a larger emblem, brand title, clock and date. The content inset is adjusted so Home and Apps remain clear of the header. The website www.shadowfoxtv.ca sits directly under the centred MORE THAN ENTERTAINMENT slogan. Amber/cyan text accents and a subtle text shadow match the ShadowFox palette. The existing Brand lettering setting still controls the main wordmark; ShadowFox colours was selected on the owner's Tanix as requested.

The owner's currently selected custom wallpaper is retained. Backgrounds remain static. The seven Exclusive Wallpapers and their assets are unchanged.

## Compatibility and data

The release signing identity, update verification, Fire TV custom-dialog compatibility, wallpaper selector and app-artwork renderer are unchanged. Existing app/user data is retained. No new permissions are requested. TV recommendation access remains read-only and optional.

## Build on Windows

Requires Python 3, a Java JDK, Android SDK platform 35 and build-tools 35.0.0. Set JAVA_HOME and ANDROID_HOME if needed. Set SHADOWFOX_SIGNING_DIR to the private directory containing the existing shadowfox-home.p12 and password.txt, then run python build_launcher_review.py.

The source archive excludes signing material, device data, test fixtures, build outputs and captures.
