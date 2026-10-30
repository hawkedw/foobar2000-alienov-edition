# Changelog

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
