# foobar2000 Alienov edition beta 0.3.5

- Add bounded automatic MilkDrop graphics-admission recovery, with a finite retry budget and coalesced display/foreground/resume triggers. Manual Retry and the existing Album Artwork fallback remain available; playback and fullscreen ownership are preserved.
- Move early native startup-window containment onto a dedicated message pump so busy main-window work does not delay the established hidden-to-embedded handoff. Exact process/generation checks and existing native plugin binaries remain unchanged.
- Fix updater helper startup identity capture: allow bounded asynchronous readiness of the observed executable path while retaining exact PID, creation-time and path checks. Failed, wrong-generation or inaccessible helpers are not accepted.
- Use one explicit **Update and restart** action to download, verify, install and restart. No second install confirmation is needed. Discovery alone does not install; cancellation before handoff, retained-payload Retry, integrity checks and rollback safeguards remain.
- Correct Telegram Connect for an existing session directory already owned by the current Windows user with Modify-only permissions. Preserve that owner while securing the private DACL; foreign ownership remains rejected and protected session data is not reset.
- Show Connecting, actionable errors and Retry directly in Telegram Account. Authorization prompts belong to Preferences; Add source becomes available only after Connected. Existing per-application session isolation, DPAPI protection and TDLib trust checks remain.

## Download

Use the complete Windows x64 portable ZIP. GitHub Code > Download ZIP is NOT the portable application.

Asset: `foobar2000-Alienov-edition-beta-0.3.5-win-x64.zip`

Size: 204316492 bytes.

SHA-256: `BF7B56C0491E1F51FA36AA1CF8F9BD266FDC0DC78D933F663B337C284220CE21`

Existing user libraries, playlists, settings and Telegram sessions remain outside the update payload. Frozen native identities and accepted factory defaults are preserved. No personal UserData, credentials or session database is included.

## Updating from beta 0.3.4

The installed beta 0.3.4 still performs this transition with its own existing controller and trusted helper. Incoming files cannot retroactively change that client's startup behavior or buttons; its existing installation confirmation and an explicit Retry may still be needed. The new one-click workflow and helper-startup correction become active after beta 0.3.5 is installed, for updates initiated by that client.

Do not unpack a clean profile over an existing installation or delete updater recovery evidence. Keep the existing profile and use its verified update/recovery path.

## Verification and remaining limitations

The combined focused regression run passed 319 tests using synthetic profiles, fake Telegram clients, controlled windows/processes and isolated WPF views. Compiled package checks confirm the three accepted changes are included, not just present in source. Both exact published beta 0.3.4 Desktop and helper contracts passed full verified extraction, manifest coverage/file hashes and transition to this exact 0.3.5 ZIP; all 1254 Frozen identities remain unchanged.

Previous bounded preview evidence includes tentative owner-positive observation of embedded MilkDrop startup and normal close. It does not establish universal absence of transient windows or real device-loss recovery in this packaged release. Actual DEVICELOST-to-device-available recovery, all graphics environments, full clean-Windows startup and complete live update download/shutdown/install/rollback/restart remain **NOT VERIFIED**. Native Direct3D can still refuse access, including after a successful preflight.

Real Telegram API authorization, phone/code/2FA, actual server rejection and successful live Add source remain **NOT VERIFIED**. Tests use fake clients and disposable data. The earlier no-credentials native load check is not a successful login. Full native authorization-modal pixel acceptance and physical mixed-DPI behavior are also unverified. Existing conservative handling of partial native initialization may require restarting the player; it does not reset stored credentials or sessions automatically.

The application remains unsigned. Existing launcher-only post-first-launch origin handling does not sign code, suppress SmartScreen, confer publisher reputation or change security policy. Font rendering remains environment-dependent.

Immutable package preparation metadata remains localOnly=true/releaseReady=false and LOCAL_ONLY_NOT_PUBLISHED/publicationAuthorized=false. Those historical preparation fields are not rewritten to imply publication; authorized publication status is recorded separately.

## Licensing and redistribution

PolyForm Noncommercial and existing third-party notices remain unchanged. Existing redistribution/source/notice restrictions remain unresolved for the legacy foobar2000 backend, WilB-derived material, SACD components, Shpeck, Winamp/MilkDrop/presets, Microsoft VC/DirectX components and FFmpeg/Chromaprint/transitive dependencies. Technical verification, noncommercial intent and owner publication approval do not confer third-party permissions. See LICENSING.md, DISTRIBUTION.md and THIRD_PARTY_NOTICES.md.
