# foobar2000 Alienov edition beta 0.3.3

- Guard MilkDrop startup with a bounded Direct3D 9 windowed-device check before native Start. Refused graphics starts show one in-panel diagnostic and Retry instead of entering the known native modal-error path. Shpeck/MilkDrop binaries remain unchanged.
- Replace two-stage Music Library setup with Choose Music Folder and Open Library Settings. Registering a Music root starts background indexing automatically; X dismisses onboarding for this launch only. Zero Music roots shows onboarding again next launch; Telegram sources do not count.
- Resume incomplete initial indexes automatically, preserving committed records and identities. Completed roots retain incremental watchers without a new full initial scan.
- Traverse sibling folders deterministically A-Z. Show throttled physical-file/logical-track counts and reliable folder/artist context in the existing status bar, without a floating progress window. Unknown totals remain indeterminate rather than displaying a fabricated percentage.
- Include updater handoff/lifetime and retained-error recovery corrections. Remove the redundant trust checkbox while retaining explicit Install and restart consent, archive integrity checks and rollback.
- Preserve playlist width corrections, sanitized Alienov factory appearance, package-local UserData, the launcher-only post-first-launch origin-mark operation and frozen native identities.

## Download

Use the complete portable release ZIP. GitHub Code > Download ZIP is NOT the portable application.

Asset: `foobar2000-Alienov-edition-beta-0.3.3-win-x64.zip`

Size: 210575489 bytes.

SHA-256: `86B26571BA9110AB169B81F4A69F8898CB1114D9C87AD9533063417E01338026`

## Acceptance and limitations

The owner confirmed working MilkDrop rendering, automatic indexing of disposable synthetic music, persisted MAIN rows, absence of onboarding after registration and normal close in an isolated current-source preview. Focused managed/SQLite tests and actual WPF render reviews cover onboarding, scan ordering/resume, progress, retry and updater regressions. The final full package is produced separately from pristine seeds, never from an executed preview profile.

The original MilkDrop code 2152 is D3DERR_DEVICELOST, not proof of insufficient VRAM. Device availability was transient on the test host; the exact external trigger remains **NOT VERIFIED**. A device loss after a successful preflight can still reach unchanged native plugin behavior. This is not a universal graphics compatibility guarantee.

The secondary onboarding route and interrupted-scan resume have focused tests but not separate owner-confirmed end-to-end GUI acceptance. A visible long-running status update under navigation, recipient Explorer behavior, clean-Windows startup and live update download/shutdown/install/rollback/restart remain **NOT VERIFIED**. Managed archive/transition compatibility does not replace these gates.

This package remains unsigned. The launcher-only origin-mark operation occurs after Windows permits the initial launch; it does not sign code, suppress SmartScreen, confer publisher reputation, change security policy or unblock updater downloads. Factory font rendering remains environment-dependent.

Immutable package preparation metadata remains localOnly=true/releaseReady=false and LOCAL_ONLY_NOT_PUBLISHED/publicationAuthorized=false. Those fields are not rewritten to imply publication; release status is recorded separately after authorized publication.

## Licensing and redistribution

PolyForm Noncommercial and existing third-party notices remain unchanged. Existing redistribution/source/notice restrictions remain unresolved for the legacy foobar2000 backend, WilB-derived material, SACD components, Shpeck, Winamp/MilkDrop/presets, Microsoft VC/DirectX components and FFmpeg/Chromaprint/transitive dependencies. Technical validation, noncommercial intent and publication approval do not confer third-party permissions. See LICENSING.md, DISTRIBUTION.md and THIRD_PARTY_NOTICES.md.
