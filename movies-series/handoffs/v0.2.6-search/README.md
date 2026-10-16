# v0.2.6 / code 8 — search-only source handoff

**NOT BUILT OR VERIFIED. The live APK/feed remains v0.2.5.**

Cloud command execution failed with `exec-server transport closed`; even `pwd` hung on repeated retries. This is a workspace runtime blocker, not a Robolectric test/dependency failure. No release build or new tests ran for this change. No v0.2.6 search APK or APK SHA-256 is available yet.

Apply to the existing v0.2.5 source root:
```
python3 apply_v026_search_fix.py /path/ShadowFoxTV_Movies_Series
```
The script stages all changes and checks every original anchor before writing. It intentionally refuses a different baseline. It does not read or write credentials, the database, artwork, updater URLs or signing keys. Package stays `ca.shadowfoxtv.movieseries`, minSdk 25; version becomes 0.2.6/code8.

Baseline source: https://raw.githubusercontent.com/gervaism-afk/shadowfox-tv-releases/main/movies-series/ShadowFoxTV-Movies-Series-0.2.5-source.zip
Compatible private source/key: canonical Library `libfile_17b47ed406a0819194026d00776861b8`, version 7, `file_00000000e65881f6b64c3bfdeeb308b4`.
Required signer SHA-256: `c018a048630b67d1b82a80308bb5e5c725fbbd7487eca6c0c461464884984e90`.

Changes:
- A local synchronous TextFieldValue owns text, caret and IME composition; delayed result state is never bound back into the editor.
- Search opening preserves the original manual-focus behavior. Closing search clears text/caret/composition/query; switching Movies/Series also clears the editor.
- Separate requested-selection flow supplies the active type immediately. Labels are Search movies / Search series.
- No poster auto-focus occurs during editor focus or for stale results. Detail return uses a single consumed navigation focus target, cleared after focus restoration succeeds. Query refreshes/grid recreation have no independent focus target.
- Existing page, count and category SQL already require the active type and are unchanged; activating search never resets the selected type.
- This handoff deliberately excludes unrelated pending mobile-touch changes.

Validation to run locally:
1. `assembleRelease`, package/code/minSdk checks, same certificate, API25 signature verification, embedded artwork, existing schema/indexes.
2. Run `testDebugUnitTest lintDebug lintRelease` if test infrastructure is available. New regressions cover slow multi-character typing across delayed results/recreated posters, caret edits, editor clear/type labels, and actual Room queries with identical MOVIE/SERIES/TV names.
3. Do not spend repeated attempts repairing Robolectric infrastructure; report any limitation and prioritize building the APK for the local physical H96 test session.
4. H96: blank editor, manual focus, slow/rapid DPAD Latin keyboard typing, caret movement and mid-word edit, return from details, hide/show search, switch type. Check lowercase `batman` against the real catalogue: 72 MOVIE rows versus 11 SERIES rows.
5. Publish APK/source/feed only under movies-series after package verification. Do not modify Platinum Player or mark a GitHub release latest.

Baseline physical observation: sequential typing sometimes works on v0.2.5; the reported focus loss was not conclusively reproduced. This change addresses the confirmed delayed binding and repeated-focus code paths.
