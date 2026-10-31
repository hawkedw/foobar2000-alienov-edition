# Changelog

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
