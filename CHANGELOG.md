# Changelog

## 0.4.3 - beta

- Close the owned legacy playback backend when exiting during playback.
- Keep the Waveform cursor and played-fill boundary visually aligned, and recover analysis after interrupted requests.
- Sort local MAIN by album artist, then by album year, album title, disc and track. Existing profiles using the old factory Year sort adopt the new default. Custom sort settings and manual playlist orders are preserved.
- Restore MAIN selection without rebuilding the visible list, and hide the player window before panel shutdown.

## 0.4.2 - beta

- Smooth the Waveform playback cursor between native position updates.
- Double-click the elapsed time to seek to a timestamp. Press Enter to apply or Escape to cancel.
- Show elapsed time above the Waveform and a fixed 0:00 at the start of the timeline.
- Show newly calculated BPM in the open MAIN playlist as results are saved.
- Improve regression coverage for playback timing, library navigation and playlist updates.

## 0.4.1 - beta

- Fix an automatic playback stop caused by mixed backend observations at the end of a track.
- In sequential playback, finish the current track before continuing from the first row of a newly opened Library Tree folder.
- Recover Biography from verified album and artist evidence when MusicBrainz is temporarily unavailable. Keep conflicting artist identities unresolved.
- Scroll the artist photo strip independently of the biography text, with hidden scrollbars and reuse of decoded thumbnails.
- Place Choose Music Folder first in the first-run setup and keep it as the primary action.
- Reopen Preferences at its last selected section, including after restarting the player.

## 0.4.0 - beta

- Biography has four layouts, with B as the default, and profile-style artist images with circle and square options.
- Biography can rotate its artist gallery, filter discography from the main text, and fall back to Wikipedia when the official Last.fm biography is unavailable.
- Library Tree navigation switches MAIN more responsively, especially when opening consecutive folders.
- Search the active playlist and the Library Tree side by side. Select a result to reveal its exact row, or use Play or Jump to from the result menu.

## 0.3.10 - beta

- Free an update slot by retiring verified, superseded update history when the retained-operation limit is reached. Active, recoverable and reusable attempts stay available.

## 0.3.9 - beta

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

## 0.3.8 - beta

- Improve durable library indexing with generation checkpoints, interruption/resume, bounded retries and root progress.
- Improve CUE handling and classify unsupported or unresolved descriptors as nonfatal skips where appropriate.
- Keep completed Library roots quiet while providing accurate scan totals, warning categories and compact diagnostics.
- Add Save full diagnostic log to export all stored diagnostic records from one consistent generation/epoch, beyond the old diagnostics page limit, without starting a scan.
- Include the accepted Telegram connection/authorization workflow, source Refresh, history indexing and Search navigation improvements.
- Preserve existing settings, playlists and Telegram sessions through the accepted update path. Keep the integrated GitHub updater and its integrity/recovery protections.
- Include Library Tree Refresh/Analysis admission fixes, forced BPM feedback, package-root AcoustID/fpcalc resolution, keyboard context-menu ownership and status-message expiry protection.

## 0.3.5 - beta

- Add bounded automatic MilkDrop graphics-admission recovery, with a finite retry budget and coalesced display/foreground/resume triggers. Manual Retry and the existing Album Artwork fallback remain available; playback and fullscreen ownership are preserved.
- Move early native startup-window containment onto a dedicated message pump so busy main-window work does not delay the established hidden-to-embedded handoff. Exact process/generation checks and existing native plugin binaries remain unchanged.
- Fix updater helper startup identity capture: allow bounded asynchronous readiness of the observed executable path while retaining exact PID, creation-time and path checks. Failed, wrong-generation or inaccessible helpers are not accepted.
- Use one explicit **Update and restart** action to download, verify, install and restart. No second install confirmation is needed. Discovery alone does not install; cancellation before handoff, retained-payload Retry, integrity checks and rollback safeguards remain.
- Correct Telegram Connect for an existing session directory already owned by the current Windows user with Modify-only permissions. Preserve that owner while securing the private DACL; foreign ownership remains rejected and protected session data is not reset.
- Show Connecting, actionable errors and Retry directly in Telegram Account. Authorization prompts belong to Preferences; Add source becomes available only after Connected. Existing per-application session isolation, DPAPI protection and TDLib trust checks remain.

## 0.3.4 - beta

- Stabilize MAIN refresh during background indexing with bounded, coalesced updates that preserve the existing presentation when rows and columns have not changed.
- Remove redundant playlist-local footers. Playlist information and indexing progress use the existing compact global status bar.
- Eliminate horizontal playlist scrolling: effective columns fit the available viewport, including vertical-scrollbar space, while preserving saved user column preferences and responsive text priorities. MAIN, custom and secondary playlist layouts share the corrected measurement behavior.
- Add independently configurable track count and total duration to the global status bar, using the full semantic playlist scope rather than only loaded viewport rows. Unknown durations and partial results remain explicit.
- Preserve indexing status priority. While indexing is active its progress takes precedence; completion restores the selected playlist's summary without an obsolete completion banner displacing it.
- Improve MilkDrop unavailable diagnostics and Retry, with the existing Album Artwork fallback when visualization cannot start. The selected native visualization binaries and audio path remain unchanged.

## 0.3.3 - beta

- Guard MilkDrop startup with a bounded Direct3D 9 windowed-device check before native Start. Refused graphics starts show one in-panel diagnostic and Retry instead of entering the known native modal-error path. Shpeck/MilkDrop binaries remain unchanged.
- Replace two-stage Music Library setup with Choose Music Folder and Open Library Settings. Registering a Music root starts background indexing automatically; X dismisses onboarding for this launch only. Zero Music roots shows onboarding again next launch; Telegram sources do not count.
- Resume incomplete initial indexes automatically, preserving committed records and identities. Completed roots retain incremental watchers without a new full initial scan.
- Traverse sibling folders deterministically A-Z. Show throttled physical-file/logical-track counts and reliable folder/artist context in the existing status bar, without a floating progress window. Unknown totals remain indeterminate rather than displaying a fabricated percentage.
- Include updater handoff/lifetime and retained-error recovery corrections. Remove the redundant trust checkbox while retaining explicit Install and restart consent, archive integrity checks and rollback.
- Preserve playlist width corrections, sanitized Alienov factory appearance, package-local UserData, the launcher-only post-first-launch origin-mark operation and frozen native identities.

## 0.3.2 - beta

- Fixed initial music-folder registration, indexing-state visibility and MAIN/Library Tree refresh. Committed partial indexes remain readable; newly registered roots report their validated availability.
- Added visible, explicitly consented root-scoped indexing progress, cancellation and targeted retry.
- Corrected Playlist Workspace column allocation: surplus viewport width fills text columns without overwriting saved widths.
- After Windows permits the user's initial launch and portable startup succeeds, remove only Internet ZoneId=3 metadata from the exact running portable launcher. Missing ADS is a no-write operation; failures are nonfatal. No recursive unblocking or changes to other files or streams.
- Preserve personal portable UserData and existing settings during upgrades, while retaining clean factory UI defaults for fresh installations.
- Keep the frozen native backend, bridge and other Frozen payload identities unchanged. The integrated consent-based GitHub updater remains included.

## 0.3.1 - beta

- Fresh factory defaults now reproduce the saved daily-driver layout and appearance.
- Playlist columns, widths, formatting, grouping, colors and panel proportions are included in clean-install defaults.
- Existing user profiles remain preserved during upgrades; this release does not silently reset personalized UI.
- The GitHub updater, explicit installation consent and rollback support remain included.
- Portable ZIP entries use canonical forward slashes; package extraction and the 0.3.0 to 0.3.1 transition pass the actual published 0.3.0 updater contract without changing updater code or payload files.

## 0.3.0 — beta, local preparation

- Canonical product title and About version: foobar2000 Alienov edition beta 0.3.0.
- Single authoritative private build version source with next patch 0.3.1.
- Fresh self-contained win-x64 managed build based on accepted Smoke05 sources.
- Narrow authorized TDLib loader update for separately pinned app-local VC runtime dependencies; original five DLLs and native-lock unchanged.
- Complete portable private payload with accepted backend, visualization stack, clean configured profile defaults and added native dependency closure.
- Local release metadata and noncommercial licensing documentation prepared. Public distribution remains blocked; no remote release exists as a result of this task.
