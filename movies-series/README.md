# ShadowFoxTV Movies & Series v0.2.3

[Download signed APK](https://raw.githubusercontent.com/gervaism-afk/shadowfox-tv-releases/main/movies-series/ShadowFoxTV-Movies-Series-0.2.3.apk) · [Updater feed](update.json) · [Verification](verification-v0.2.3.json)

Package `ca.shadowfoxtv.movieseries`, version code 5, Android TV 10+. Compatible signer retained. Install over the existing app; do not uninstall. Existing updater users can open Settings > App updates. v0.2.0 needs this manual bootstrap installation.

Large-catalogue browsing now uses compound database indexes, page changes avoid repeating filter counts, and import entity batches are bounded. First launch creates indexes once. Accounts, saved items and progress are retained by the index-only migration. Final TV artwork and Tanix stability changes remain.

Prior build validation passed 100 unit tests, 120 host SQLite scenarios and debug/release lint with zero errors (73 warnings per variant). Recovery checks reconfirmed the exact APK checksum, compatible certificate, package/version, CRC and both new index definitions. Device performance remains untested; host timings are not TX96 measurements.

The final source upload was interrupted and the saved checkpoint is incomplete. Source handoff is pending recovery; [v0.2.2 source](ShadowFoxTV-Movies-Series-0.2.2-source.zip) remains available as an older version and does not represent this APK. Attribution: SERFF/iptv-app, Apache 2.0; see LICENSE.

This is an isolated Movies & Series feed; Platinum Player releases are unchanged.
