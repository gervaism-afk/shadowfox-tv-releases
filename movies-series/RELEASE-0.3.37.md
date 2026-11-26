# ShadowFoxTV Movies & Series 0.3.37

[Signed repair APK](ShadowFoxTV-Movies-Series-0.3.37.apk) · [Complete source](ShadowFoxTV-Movies-Series-0.3.37-source.zip) · [Updater feed](update.json) · [Verification](verification-0.3.37.json)

Fixes a false “Update signing certificate mismatch” on the user's Android 9/API 28 Fire
Stick. The installed 0.3.29 and the public update have the same original signing key.
The device's PackageManager returns no archive SigningInfo when only the modern
certificate flag is requested. This was reproduced against its own installed APK,
and public 0.3.36 using a temporary shell-only reader.
Requesting both modern and legacy flags returns the actual matching certificate.

**One-time repair:** affected old updater versions cannot install their own fix. Download
this signed APK and install it as a normal update over the existing app, retaining
its saved login/data. After this bootstrap, future updater checks use the compatible
lookup. Installation is left to the user; no app was installed, uninstalled, opened
or cleared during this repair task. No security check or Android protection is disabled.

The updater requests both flags on API 28+, and the supported legacy flag on API 25–27.
It prefers the current signer set and uses actual legacy metadata only when modern
data is absent. It never switches to legacy metadata to hide a mismatching modern
signer. Empty/missing, different or additional signer sets still fail. SHA256/size,
trusted URL, package and increasing-version guards are unchanged. Unreadable certificate
metadata now has a separate message from a genuine certificate mismatch.

287 tests passed with zero failures; release lint has zero errors.
New regression cases cover flags for each API family, missing modern metadata,
unreadable data, contradictory metadata, and wrong/extra signer sets. The final signed
APK's package/API/ARMv7 compatibility and original certificate were verified. On the
actual Fire Stick, the fixed flags read the installed 0.3.29 and public 0.3.36
certificates; the old flags reproduce the failure. The device went offline before
the final 0.3.37 archive recheck. Its original certificate was verified on the build
host; final installation and native verification remain pending. Temporary APK/helper/ART files were removed. No app UI,
audio/system/display/server/key settings or saved preferences were changed. Actual
installation and a subsequent in-app update remain for the user to perform.

Only the version and UpdateController change from the current 0.3.36 source, with a small
UpdateCertificates helper and six regression tests added. Account storage/schema,
database, resources/original logo, Cobalt/default/saved theme behavior, About credit,
Home focus, player and orientation are byte-unchanged. Package `ca.shadowfoxtv.movieseries`,
code 49, Android 7.1/API 25 or newer. Original signing identity retained. Complete source
excludes private signing keys/local configuration and retains attribution/licences.
