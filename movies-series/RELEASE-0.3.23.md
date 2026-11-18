# ShadowFoxTV Movies & Series 0.3.23

[Signed APK](ShadowFoxTV-Movies-Series-0.3.23.apk) · [Complete source](ShadowFoxTV-Movies-Series-0.3.23-source.zip) · [Updater feed](update.json) · [Verification](verification-0.3.23.json)

Restores the exact original full ShadowFoxTV Movies & Series logo, including its fox, filmstrip, lettering and colours. The redesigned mark introduced in 0.3.22 is removed from every in-app surface and the Android 12 startup override. The original loading-screen layout is restored. The requested Settings gear remains.

The unchanged highest-resolution original image (320x320) is loaded as a density-independent bitmap rather than allowing Android to select the smaller copies. Inside scaling avoids enlarging it beyond its available pixels. The source image is byte-identical to the original artwork: SHA256 `84572ab2bce1f453b8b72e4329fc3334d6160621dbfb8410e3180575ad2013f9`. There is no redraw, retouch or AI replacement. Launcher icons and banners remain unchanged.

254 existing automated checks passed; release lint has no errors. Original artwork bytes and the removal of the rejected resources were audited against the original source. The exact signed APK was installed and hash-verified on Tanix. Original Home/library branding, the gear's remote focus/Settings/Back path, retained Adult visibility control and installed version were checked. No preferences were edited or provider playback started; no physical-phone playback tested.

Saved logins, Adult visibility and filtering, history, themes, Home layout, continuous paging, player/native audio, orientation, database and updater are retained. The correction changes image selection/scaling, keeps the existing gear renderer, and removes the rejected artwork. Earlier Tanix 4K/heat issue remains unresolved; no playback or thermal changes are claimed.

Package `ca.shadowfoxtv.movieseries`, version code 35, Android 7.1/API 25 or newer. Install over the existing app to retain data. Signed with the original compatible certificate. This feed is separate from Platinum Player.

Complete source retains the original attribution, bundled Inter/OFL fonts, AndroidX Media3/FFmpeg source, four-ABI audio libraries and licences. Private signing keys and local configuration are excluded.
