# ShadowFoxTV Movies & Series 0.3.13

[Download signed APK](ShadowFoxTV-Movies-Series-0.3.13.apk) · [Complete source checkpoint](ShadowFoxTV-Movies-Series-0.3.13-source.zip) · [Updater feed](update.json) · [Verification](verification-0.3.13.json)

DTS playback now uses an audio-only software decoder while video stays on hardware. Stream info is available in the normal playback controls for TV remote and touch, with a focused Close button. Playback actions wrap on narrow phones. This avoids relying on the Tanix blue key, which also opens its manufacturer's Apps screen.

Keeps the Apple TV inspired interface, redesigned Settings without About, provider-derived movie/series categories, saved accounts, library, watch progress, updater and existing phone/TV orientation policy. Categories are grouped only when recognized provider labels exist; original provider groups remain selectable. Existing kids-profile visibility settings apply.

Package `ca.shadowfoxtv.movieseries`, version code 25, Android 7.1/API 25 or newer. Install over the existing app to retain your data. Signed with the original compatible certificate. This update feed is isolated from Platinum Player.

178 automated tests passed; release lint has no errors. Tanix checks covered DTS stereo, DTS six-channel, AAC, resume, touch/remote Stream info, category scopes and Settings. The installed final APK hash matches this download. Physical speaker audibility was not confirmed. The device temperature peaked at 85.274 C during these checks; no reboot was observed. The earlier 4K Tigerdump cause remains unresolved; this release's device checks used 1080p AVC samples.

The complete source checkpoint includes four-ABI native audio libraries, FFmpeg source, provenance and licenses. It is based on the published redesigned 0.3.10 source; the documented 0.3.11 and 0.3.12 changes were restored because their source checkpoints were not published. Private signing keys and local configuration are excluded.

Based on SERFF/iptv-app and AndroidX Media3 (Apache 2.0). FFmpeg 6.1.6 is used under LGPL 2.1 or later; its license and source are included. Original project attribution and LICENSE are retained.
