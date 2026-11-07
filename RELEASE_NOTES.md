# foobar2000 Alienov edition beta 0.3.9

- Reuse a compact playback sequence so Shuffle, Next and Previous can move through large playlists with less work.
- Speed up Library Tree to MAIN navigation by querying the selected folder scope and cancelling obsolete requests.
- Prepare playlist pages before following distant playback jumps, keep the viewport populated, and reveal the last row within the bottom edge.
- Keep MAIN navigation responsive and follow the playing row when using Next after changing folders.
- Play the selected track from the toolbar after stopping. Double-clicking a visible row leaves the scroll position in place.
- Restore missing generated external CUE files on playback when the original sources and track boundaries can be verified.
- Check for updates in the background at portable startup and download compatible packages automatically. The centered status indicator shows progress, offers Retry on failure and enables Close Player to Update after verification. Existing opt-outs are respected.
- Use the compact Default and Shuffle buttons next to Stop. Choose among B1–B4 icon pairs in Appearance Constructor. Other playback orders remain available from the Playback Order menu.
- Read bundled release history offline in Help → What's New.
- In the green theme, the playing row uses white for number, duration, artist and codec. Title and album stay green. Other themes use their own colors.

## Portable update and compatibility

Beta 0.3.8 and 0.3.9 both use library schema 33. The updater preserves the portable profile and library. Keep a consistent backup before updating. Existing themes load without rewriting, and saved B2–B4 theme options may be unfamiliar to older versions.

The package is unsigned. Clean Windows installations, physical mixed-DPI behavior and exhaustive native or Telegram scenarios remain NOT VERIFIED. Existing third-party notices and redistribution limitations apply. See THIRD_PARTY_NOTICES.md and LICENSING.md.
