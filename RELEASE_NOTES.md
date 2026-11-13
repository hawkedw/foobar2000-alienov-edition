# foobar2000 Alienov edition beta 0.4.4

- MAIN opens at the first row when you select a different folder in Library Tree. Selecting the same folder keeps your scroll position.
- Single-folder MAIN queries do less work in SQLite by skipping duplicate elimination where the query branches cannot overlap.
- A bounded first-page cache lets MAIN return to previously visited, unchanged folders without showing Loading on a valid cache hit. The first visit to a large folder can still take about 1–2 seconds in the tested setup.

AlbumChronology, playback, Search, custom playlists, session restoration and the existing update behavior are preserved.

## Portable update

The trusted updater from beta 0.4.3 applied this package in a disposable installation. Library schema 33, settings, layouts, playlists, selection and Biography data were preserved. Before updating your own installation, close the player and make a complete backup of the portable directory, including its profile. Reopen 0.4.3, check for updates and follow the in-app prompt. For a fresh install, extract the complete portable ZIP into its own folder.

## Known limitations

A transient native MilkDrop/Shpeck title bar may appear during startup. The existing MilkDrop activation test failure was also reproduced against published beta 0.4.2.

The Windows x64 application is unsigned. Clean-Windows and real-library acceptance remain NOT VERIFIED. The bundled Last.fm application key is extractable. Existing third-party redistribution, corresponding-source and notice obligations still apply.
