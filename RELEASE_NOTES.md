# foobar2000 Alienov edition beta 0.4.5

- MAIN renders rows with less work during folder changes and scrolling. Playback following no longer cancels a pending MAIN page before a valid replacement is ready.
- Warm Library Tree revisits can show the correct first rows without Loading. Cold navigation and Shuffle Next do less SQLite work for eligible scopes while preserving order and track identities.
- Generated CUE descriptors now live in the hidden .FoobarCueCache directory inside the configured music root. Selecting an indexed CUE track can regenerate a missing descriptor using the original audio.
- After the portable updater applies 0.4.5 over 0.4.4, the first launch checks configured volumes for verified obsolete CUE cache files. An active native backend or filesystem lock defers removal. Unrecognized files and renamed directories are preserved.

On the first launch after this update, playback starts stopped. A saved native technical row may still refer to an old CUE. Select the track in MAIN to regenerate its playback descriptor. Ordinary playback controls then work on the newly opened track.

First visits can still load from SQLite. The navigation cache remains session-local. Back up the entire closed portable installation before updating. This update uses the existing library schema and native engine. The application is unsigned. A transient native MilkDrop/Shpeck title bar may appear during startup. Clean-Windows acceptance remains unverified, and existing third-party terms still apply.

Automatic removal of the obsolete CUE cache at the root of a physical volume during a complete upgrade remains NOT VERIFIED. Cleanup passed filesystem tests in disposable directories on physical volumes. Third-party redistribution, corresponding-source and notice obligations remain in force.
