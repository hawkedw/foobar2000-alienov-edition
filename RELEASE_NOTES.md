# foobar2000 Alienov edition beta 0.3.4

- Stabilize MAIN refresh during background indexing with bounded, coalesced updates that preserve the existing presentation when rows and columns have not changed.
- Remove redundant playlist-local footers. Playlist information and indexing progress use the existing compact global status bar.
- Eliminate horizontal playlist scrolling: effective columns fit the available viewport, including vertical-scrollbar space, while preserving saved user column preferences and responsive text priorities. MAIN, custom and secondary playlist layouts share the corrected measurement behavior.
- Add independently configurable track count and total duration to the global status bar, using the full semantic playlist scope rather than only loaded viewport rows. Unknown durations and partial results remain explicit.
- Preserve indexing status priority. While indexing is active its progress takes precedence; completion restores the selected playlist's summary without an obsolete completion banner displacing it.
- Improve MilkDrop unavailable diagnostics and Retry, with the existing Album Artwork fallback when visualization cannot start. The selected native visualization binaries and audio path remain unchanged.

## Download

Use the complete Windows x64 portable ZIP. GitHub Code > Download ZIP is NOT the portable application.

Asset: `foobar2000-Alienov-edition-beta-0.3.4-win-x64.zip`

Size: 204300548 bytes.

SHA-256: `C0C5EB9614766A8BE50CA813085DA0EA59DEEC0C2B993B600513DACF126A41F0`

Existing UserData, playlists, settings and Telegram sessions remain outside update payloads. Factory defaults remain install-only-if-absent; frozen native identities are preserved.

## Verification and limitations

The existing 416 focused managed/SQLite/WPF tests and isolated rendered reviews cover the scoped playlist layout, indexing refresh and global-status changes. This publication preparation reuses those results without rebuilding the player or repeating that suite.

Both exact published beta 0.3.3 Desktop and helper updater contracts have passed verified extraction of this exact ZIP, full manifest coverage and file hashes, and the 0.3.3 to 0.3.4 transition with all 1254 Frozen files unchanged. The archive contains no personal UserData, library database, playlists or account sessions. These are package-contract checks, not a live update installation.

Native MilkDrop Direct3D recovery remains **NOT VERIFIED on the affected PC**. Unavailable/Retry/fallback presentation and managed guards do not establish native device recovery or prove that all graphics problems are fixed. A device loss after admission can still reach unchanged native plugin behavior.

Full clean-Windows startup, continuous real-library indexing/navigation behavior, physical mixed-DPI behavior and real update download/shutdown/install/rollback/restart remain **NOT VERIFIED** for this candidate. The optional 50,000-item scale gate was not run. Isolated WPF renders and package contracts do not replace those acceptance gates.

The application is unsigned. Existing launcher-only post-first-launch origin handling does not sign code, suppress SmartScreen, confer publisher reputation or change security policy. Factory font rendering remains environment-dependent.

Immutable package preparation metadata remains localOnly=true/releaseReady=false and LOCAL_ONLY_NOT_PUBLISHED/publicationAuthorized=false. Those historical preparation fields are not changed to imply publication; any authorized publication status is recorded separately.

## Licensing and redistribution

PolyForm Noncommercial and existing third-party license/notices remain unchanged. Existing redistribution/source/notice restrictions remain unresolved for the legacy foobar2000 backend, WilB-derived material, SACD components, Shpeck, Winamp/MilkDrop/presets, Microsoft VC/DirectX components and FFmpeg/Chromaprint/transitive dependencies. Technical validation, noncommercial intent and owner publication approval do not confer third-party permissions. See LICENSING.md, DISTRIBUTION.md and THIRD_PARTY_NOTICES.md.
