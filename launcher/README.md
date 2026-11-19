# ShadowFoxTV Launcher Pro 2.4.0

Version code 41 · package `com.shadowfox.tvlauncher.review`.

## Local weather

A weather pill sits on the right, in line with Home and Apps. Its rounded material, height, typography, colour accents and focus fill match the navigation banner. It shows the area, a vector condition icon, temperature and condition text. The widget remains available on both Home and Apps. Right from Apps reaches weather, OK opens weather options, and Down enters the app rows.

Automatic (ISP) is the default. The device requests its approximate area using its own public-IP connection through GeoJS. Coordinates are rounded to two decimal places before weather lookup; the public IP returned by the service is not persisted. The widget says Near the detected area. A network change triggers another lookup with a one-minute cooldown; normal foreground checks use a six-hour location cache. A VPN may change the detected area. No GPS or Android location permission is requested.

Weather location offers Automatic (ISP) or a manual city/postal-code search with a choice of matching results. Celsius is the default; Fahrenheit is also available. Weather options are available from the widget or Settings → Home screen → Local weather. Weather sources and licence links are available inside its menu.

Weather forecasts are fetched off the UI thread, use HTTPS and the system certificate trust store, identify this app with its public website, support gzip and bounded HTTPS redirects, and cache data across launches. Forecasts refresh no more often than every three hours and respect a later server expiry. Conditional requests use Last-Modified. Up to eight selected locations retain forecast caches. Cached hourly forecasts advance locally; old or malformed data displays as unavailable. Failed automatic updates back off, and users can retry from the menu. Foreground timers stop when the launcher leaves the screen. No media recommendations or Quick launch content are restored.

## Weather sources

Forecast: [MET Norway](https://api.met.no/weatherapi/locationforecast/2.0/documentation), [CC BY 4.0 and data policy](https://docs.api.met.no/doc/License.html). Temperatures are rounded and condition labels/icons are adapted for ShadowFox. Global forecast refresh intervals follow the provider documentation.

Automatic location: [GeoJS](https://www.geojs.io/) using MaxMind GeoLite2. API reference: https://www.geojs.io/docs/v1/endpoints/geo/ . This is approximate public-IP geolocation, not GPS.

Manual location search: [Photon](https://github.com/komoot/photon) / [© OpenStreetMap contributors, ODbL](https://www.openstreetmap.org/copyright). Searches happen only after the user presses Search. Repeated identical queries use a seven-day local cache. There is no request-on-typing autocomplete.

## Existing launcher

The enlarged branded header, www.shadowfoxtv.ca, selected wallpaper, free-floating artwork, app names, order, assignments and category filters remain in use. Your apps remains near the bottom of the first viewport; Recently opened stays below it. The seven Exclusive Wallpapers and image resources are unchanged.

Update signing identity, APK/certificate validation, Fire TV dialog compatibility, wallpaper selector and icon renderer implementations are unchanged. Existing app data is retained and no new permissions are requested.

## Build on Windows

Requires Python 3, a Java JDK, Android SDK platform 35 and build-tools 35.0.0. Set JAVA_HOME and ANDROID_HOME if needed. Set SHADOWFOX_SIGNING_DIR to the private directory containing the existing shadowfox-home.p12 and password.txt, then run python build_launcher_review.py.

The source archive excludes signing material, cached weather/location data, device preferences, test fixtures, build outputs and captures.
