# ShadowFoxTV Movies & Series v0.2.4

[Download signed APK](ShadowFoxTV-Movies-Series-0.2.4.apk) · [Download source](ShadowFoxTV-Movies-Series-0.2.4-source.zip) · [Update feed](update.json) · [Verification](verification-v0.2.4.json)

Adds a standard Android launcher entry so the installed app appears in phone and tablet app drawers. The Android TV launcher entry remains. The existing interface opens in landscape; this is not a portrait UI redesign.

Package `ca.shadowfoxtv.movieseries`, version code 6, Android 10+. Install over the existing app without uninstalling. Existing updater users can open Settings > App updates. Android confirms installation. v0.2.0 users need one manual bootstrap install.

Compatible signer, TV artwork, index-only database migration, bounded import batches and Tanix performance fixes are retained. Accounts, saved items and playback progress are not intentionally reset. First launch after v0.2.2 creates catalogue indexes once.

Source is based on SERFF/iptv-app, Apache 2.0. Original attribution and LICENSE are retained. Public source excludes signing keys and local.properties. Official compatible updates require the privately retained signing key. This channel is isolated from Platinum Player.

Build validation and package checks are recorded in verification-v0.2.4.json. Physical phone/TV testing has not been performed here.
