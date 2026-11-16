# Movies & Series 0.3.14 — Continuous browsing

Movies, Series, search and My List now scroll continuously. Titles load in small
batches with a bounded cache; Next/Previous page buttons are removed.

Remote navigation has explicit paths between the header, categories and titles.
Returning from a title restores its focus; returning from Settings retains the
library position and restores focus to Settings. Search completion enters results.
Phone touch browsing remains supported.

Adult movies/series have a visible shortcut near the top of the library and
Categories picker in ordinary profiles. If the provider has not supplied matching
categories, the section explains this instead of disappearing. No titles are
invented or reassigned by their names. Existing kids-profile filtering remains.

Profiles is removed from Settings. Settings now has Account, Playback, Library
and Updates. Existing stored accounts, profiles, watch progress, database schema,
player, updater and phone/TV orientation policy are retained.

Package ca.shadowfoxtv.movieseries, version code26. Install over the existing app
with the original signing identity to retain your data.
