# foobar2000 Alienov edition beta 0.3.2

- Fixed initial music-folder registration, indexing-state visibility and MAIN/Library Tree refresh. Committed partial indexes remain readable; newly registered roots report their validated availability.
- Added visible, explicitly consented root-scoped indexing progress, cancellation and targeted retry.
- Corrected Playlist Workspace column allocation: surplus viewport width fills text columns without overwriting saved widths.
- After Windows permits the user's initial launch and portable startup succeeds, remove only Internet ZoneId=3 metadata from the exact running portable launcher. Missing ADS is a no-write operation; failures are nonfatal. No recursive unblocking or changes to other files or streams.
- Preserve personal portable UserData and existing settings during upgrades, while retaining clean factory UI defaults for fresh installations.
- Keep the frozen native backend, bridge and other Frozen payload identities unchanged. The integrated consent-based GitHub updater remains included.

## Download

Use the complete portable release ZIP. GitHub Code > Download ZIP is NOT the portable application.

Asset: `foobar2000-Alienov-edition-beta-0.3.2-win-x64.zip`

Size: 204261616 bytes.

SHA-256: `7B2C452C94EF9F1559D3D46BD67732A311F0AA8637A03B5122513227806CA1C3`

## Acceptance and Windows security limitations

Actual downloaded-client startup, full update download/shutdown/installation/rollback/restart, recipient Explorer warning behavior and clean-Windows acceptance are **NOT VERIFIED**. Focused tests and package/manifest/updater-contract validation do not replace these gates. Existing factory font preferences remain environment-dependent.

The launcher-only operation runs after the initial Windows execution decision. It does not provide an Authenticode signature, suppress SmartScreen, create publisher reputation, bypass a security block or override security policies. This accepted package remains unsigned. Restricted/unsupported/denied metadata operations are retained or fail nonfatally without elevation.

The immutable package retains its preparation metadata (`runtime-manifest.json`: localOnly=true, releaseReady=false; packaged release.json: LOCAL_ONLY_NOT_PUBLISHED, publicationAuthorized=false). Those fields were not edited to claim acceptance; public release status is recorded separately by GitHub and repository metadata after authorized publication.

## Licensing and redistribution

PolyForm Noncommercial and existing third-party notices remain unchanged. Existing third-party redistribution/source/notice restrictions remain unresolved for the legacy foobar2000 backend, WilB-derived material, SACD components, Shpeck, Winamp/MilkDrop/presets, Microsoft VC/DirectX components and FFmpeg/Chromaprint/transitive dependencies. Technical validation, noncommercial intent and publication approval do not confer third-party permissions. See LICENSING.md, DISTRIBUTION.md and THIRD_PARTY_NOTICES.md.
