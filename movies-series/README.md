# ShadowFoxTV Movies & Series v0.2.2

Standalone Android TV Movies & Series app. This channel is separate from Platinum Player; its releases and latest-release tag are unchanged.

- [Download signed APK](https://raw.githubusercontent.com/gervaism-afk/shadowfox-tv-releases/main/movies-series/ShadowFoxTV-Movies-Series-0.2.2.apk)
- [Download source ZIP](https://raw.githubusercontent.com/gervaism-afk/shadowfox-tv-releases/main/movies-series/ShadowFoxTV-Movies-Series-0.2.2-source.zip)
- [Updater metadata](update.json)
- [Build verification](verification-v0.2.2.json)
- [SHA-256 checksums](SHA256SUMS)

Package `ca.shadowfoxtv.movieseries`, version code **4**, Android TV 10+. Same compatible signing certificate as v0.2.0 and v0.2.1.

**v0.2.0 needs one manual bootstrap installation.** Install this APK over the existing app; do not uninstall. Your account, database and progress are retained. Later updates are checked at launch and in Settings > App updates. Android may require permission to install unknown apps and confirms installation.

Final Android TV artwork is integrated; all 30 embedded brand PNGs match the supplied pack in visible pixels, alpha and dimensions. Legacy and adaptive launchers are verified; old launcher/banner resources are removed. Tanix stability changes are retained. **95 unit tests pass, debug/release lint have zero errors (73 warnings each).** Physical Tanix playback/installer testing remains to be completed.

Updater downloads verify exact size, SHA-256, package, higher version code and the installed signing certificate before Android installation. Public source excludes signing keys and local.properties; use the compatible privately held key to build official updates. Source is based on SERFF/iptv-app (Apache 2.0); attribution and LICENSE are retained in the source archive.
