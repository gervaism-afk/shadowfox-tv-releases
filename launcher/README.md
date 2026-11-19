# ShadowFoxTV Launcher Pro 2.5.0

Version code 42 · package `com.shadowfox.tvlauncher.review`.

## Saved categories on Home

Home now renders each nonempty saved category as its own floating app row. The category names, order and app assignments come directly from the existing settings. The first nonempty category sits near the bottom of the landing viewport; the remaining category rows follow below it in saved order. Recently opened follows the category rows. Apps are no longer combined into one aggregate Home row. No reset or migration of the user's categories is required.

Rows use the same artwork, labels, transparency, focus treatment and app options as before. D-pad Down/Up moves between rows, and Back restores the landing page. The Apps page still provides the complete library and category filters. Empty categories remain in category settings until apps are assigned.

## Expanded Exclusive Wallpapers

ShadowFox Exclusive Wallpapers now contains 39 backgrounds: the previous seven plus 32 distinct images from the owner's Tanix Pictures/Wallpapers folder. Six exact duplicate files were merged; all distinct images and variants are retained. Existing entry IDs and order are unchanged. The added entries have stable IDs and descriptive names.

Full-size PNG copies use high-quality WebP without resizing or cropping. Full-image and central-logo luminance SSIM checks at display resolution meet a minimum 0.99, with alpha verified unchanged. Images that do not meet that threshold retain lossless encoding. The original files remain untouched on the device and in the local backup. JPEGs remain in their original format. Dedicated small thumbnails keep browsing responsive. Larger previews decode off the UI thread; cancelled previews cannot replace a later selection. The Home background decoder samples large resources to the display size to limit bitmap memory use. The source images are not creatively modified.

Browsing remains a preview until Apply wallpaper is selected. Back cancels. The owner's currently selected custom background is retained during the update. Wallpaper originals and previews are bundled for offline use; the gallery does not depend on the source folder staying on the device.

## Existing launcher

The 2.4.0 automatic ISP weather widget, its location/temperature settings, website header, app artwork, transparency controls and app management remain in use. No media recommendation, Continue watching or Quick launch rows are restored. The existing update signing identity, APK/certificate verification, Fire TV dialog compatibility and permissions are unchanged.

Weather forecast: [MET Norway, CC BY 4.0](https://docs.api.met.no/doc/License.html). Automatic ISP area: [GeoJS](https://www.geojs.io/) / MaxMind GeoLite2. Manual city search: [Photon](https://github.com/komoot/photon) / [OpenStreetMap contributors, ODbL](https://www.openstreetmap.org/copyright). Weather sources and credits remain available inside the widget options. ISP location is approximate and may follow a VPN exit location.

## Build on Windows

Requires Python 3, a Java JDK, Android SDK platform 35 and build-tools 35.0.0. Set JAVA_HOME and ANDROID_HOME if needed. Set SHADOWFOX_SIGNING_DIR to the private directory containing the existing shadowfox-home.p12 and password.txt, then run python build_launcher_review.py.

The source archive excludes signing material, cached weather/location data, device preferences, test fixtures, build outputs and captures.
