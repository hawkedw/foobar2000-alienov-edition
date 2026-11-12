# foobar2000 Alienov edition beta 0.4.3

- Close the owned legacy playback backend when exiting during playback.
- Keep the Waveform cursor and played-fill boundary visually aligned, and recover analysis after interrupted requests.
- Sort local MAIN by album artist, then by album year, album title, disc and track. Existing profiles using the old factory Year sort adopt the new default. Custom sort settings and manual playlist orders are preserved.
- Restore MAIN selection without rebuilding the visible list, and hide the player window before panel shutdown.

## Portable update

Beta 0.4.2 uses the trusted portable updater. The update keeps existing schema-33 Library data, settings, layouts, playlists and Biography cache. An old custom sort identical to the former factory Year sort is interpreted as the factory setting.

## Known limitations

A transient native MilkDrop/Shpeck title bar may appear during startup, including when Album Artwork is selected.

The application is unsigned. Clean-Windows acceptance remains NOT VERIFIED. The bundled Last.fm application key is extractable. Existing third-party redistribution, source and notice conditions still apply.
