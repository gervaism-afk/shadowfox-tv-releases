# Movies & Series 0.3.5 — Cinema polish and fresh discovery

A more cinematic Home with atmospheric artwork, correctly proportioned TV posters, champagne accents, refined typography, shared navigation and clearer focus states. Phones have directly accessible Settings and responsive navigation; library, details and account setup use the same visual language.

Home no longer always opens on the first catalogue titles. Fresh sessions and launcher reopens advance the spotlight and discovery shelves through the eligible collection. Use New picks for an immediate change. Returning from details/playback and rotating a phone retain the current picks. My List and Continue Watching retain their existing order.

At most 24 discovery entries per type are materialized; there is no whole-catalogue object load or random SQL sort. Profile/kids filters apply. Database schema, saved provider credentials, player and updater implementations are retained. Install as an update without uninstalling.

Validation: 142 unit/Compose tests passed; release lint has zero errors. TV/phone emulator layout checks passed. Google TV Streamer was updated in place and verified for New picks, changing spotlight on launcher reopen, and retaining picks on detail return. Real provider playback was not exercised. Synthetic layout-test titles/artwork are not bundled with the app.
