# ShadowFoxTV Movies & Series 0.3.8 (20)

Fixed the first-run TV welcome layout so the complete QR code and phone-setup URL fit at 1080p. The setup panel can take remote focus and scroll into view with larger text. Phone portrait onboarding retains its touch layout.

Fixed a phone-form handoff after visiting Settings and returning to Welcome: only the visible Settings screen now consumes submissions. Existing settings load before applying the received draft. Receiving a form does not save it automatically.

Validation: 152 automated tests passed and release lint has no errors. Local Android TV checks covered the full QR/link, remote focus, phone handoff, connection testing, explicit Save, Home/library poster focus after details, search typing/Back, Series, My List, and Settings return paths. The APK retains the original signing identity; an in-place local update preserved its fixture account.

The physical streamer remains on 0.3.7 while in use, as requested. 0.3.8 was tested on a local emulator with fictional catalogue data. Real provider playback was not exercised.

Saved account persistence, player, updater, database schema, cinematic Home/discovery, Settings keyboard fixes, portrait support and touch controls are retained. Install over the existing app. Checksums and source accompany the APK.
