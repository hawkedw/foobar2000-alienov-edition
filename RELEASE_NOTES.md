# foobar2000 Alienov edition beta 0.4.1

- Fix an automatic playback stop caused by mixed backend observations at the end of a track.
- In sequential playback, finish the current track before continuing from the first row of a newly opened Library Tree folder.
- Recover Biography from verified album and artist evidence when MusicBrainz is temporarily unavailable. Keep conflicting artist identities unresolved.
- Scroll the artist photo strip independently of the biography text, with hidden scrollbars and reuse of decoded thumbnails.
- Place Choose Music Folder first in the first-run setup and keep it as the primary action.
- Reopen Preferences at its last selected section, including after restarting the player.

## Portable update

Beta 0.4.0 can update through the trusted portable updater. The update preserves the existing schema-33 Library, preferences, playlists and Biography cache. The packaged Last.fm application key is extractable and is separate from account credentials.

This release is unsigned. Clean-Windows acceptance remains NOT VERIFIED. Biography depends on provider availability and sufficient identity evidence. Existing third-party redistribution, source and notice conditions still apply.
