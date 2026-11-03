# Movies & Series 0.3.6 — Settings remote scrolling fix

Fixed the TV Settings scroll trap reproduced on Google TV Streamer: moving focus into account text fields opened the keyboard and intercepted further Down presses.

TV fields are now focusable summaries. Press OK to deliberately open a single-field editor; Done applies the edit to the form and Cancel discards the draft. The account Save action retains its existing behavior. Phone/tablet direct editing and password masking are retained.

Settings and Back stay pinned above a bounded scrolling viewport, a subtle scroll indicator shows position, and the final About block is reachable with D-pad focus.

Installed and verified on Google TV Streamer: 24 Down presses reached About without opening an editor, the header stayed visible, and explicitly editing/cancelling returned to Settings. No typing, saving, or account changes were performed during device validation. 146 unit/Compose tests pass; release lint has zero errors. Database, source-account persistence, player, Home discovery and updater implementations are unchanged. Install over the existing app without uninstalling.
