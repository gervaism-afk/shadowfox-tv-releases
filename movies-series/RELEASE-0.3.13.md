# Movies & Series 0.3.13 (code 25)

Adds an audio-only FFmpeg extension for DTS, AC-3 and E-AC-3. The renderer
prefers decoded PCM over compressed passthrough advertised by boxes whose
audio output cannot initialize. Video and AAC retain platform decoding.

Stream info is available in the normal playback controls, with a focused
Close button. This avoids relying on the Tanix blue key, which also opens
the manufacturer's Apps screen. Touching the video opens playback controls;
the action buttons wrap on narrow phones.

The public 0.3.10 redesigned source checkpoint is the source baseline.
The subsequent 0.3.11 and 0.3.12 releases published APKs without their source
checkpoints. Their documented changes are restored here: Settings has no
About category, and Movies/Series have a scrollable Categories picker with
provider-derived grouped genres plus the original provider groups. Adult
groups open directly in ordinary profiles; existing kids-profile filtering
continues to apply. Search, counts and pagination are scoped to the active
content type and genre groups.

Account storage, database schema, updater and phone/TV orientation policy
are unchanged from the published source baseline. Install over the existing
app with the original signing identity to retain saved account and library.

Native decoder source provenance, build configuration and licenses are in
`media3-ffmpeg/NATIVE-BUILD.md`. The source checkpoint includes all four ABI
libraries and the original FFmpeg source archive. It excludes private signing
keys and local configuration.
