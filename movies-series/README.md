# ShadowFoxTV Movies & Series v0.2.5

[Download single APK](ShadowFoxTV-Movies-Series-0.2.5.apk) · [Source ZIP](ShadowFoxTV-Movies-Series-0.2.5-source.zip) · [Updater feed](update.json) · [Verification](verification-v0.2.5.json)

Supports Android 7.1/API 25 and newer, including the Android compatibility level of Fire TV Stick 4K first generation / Fire OS 6. v0.2.4 required Android 10/API 29 and cannot install on that device. The APK includes 32-bit ARM native libraries and both mobile and Android TV launcher entries. Existing landscape interface retained.

This release backports date/time APIs and guards newer package certificate, version and install-permission APIs in the updater. Size, SHA-256, package, higher version and certificate verification remain mandatory on older devices. Physical Firestick installation and playback remain to be confirmed by the user.

Package `ca.shadowfoxtv.movieseries`, version code 7. Install over the existing app; do not uninstall. Existing updater users can use Settings > App updates. v0.2.0 users need one manual bootstrap update. Fire OS must allow installation from the chosen installer; Android/Fire OS confirms installation.

Final TV artwork, Tanix stability settings, bounded import batches and indexed library browsing are retained. Database schema 18 is unchanged. Source excludes signing keys and local.properties; official updates require the privately retained compatible key.

Source based on SERFF/iptv-app (Apache 2.0); original attribution and LICENSE retained. This Movies & Series updater feed is isolated from Platinum Player.
