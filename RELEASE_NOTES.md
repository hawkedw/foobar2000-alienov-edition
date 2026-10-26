# foobar2000 Alienov edition beta 0.3.0

Prepared metadata: repository `hawkedw/foobar2000-alienov-edition`, tag `v0.3.0`, release type **Pre-release**, channel `beta`. Intended single complete asset: `foobar2000-Alienov-edition-beta-0.3.0-win-x64.zip`, accompanied by SHA256SUMS.txt.

Status: private local development candidate. Nothing has been uploaded or publicly released. Redistribution permissions for required third-party material are unresolved, and this task expressly prohibits all remote operations.

The managed build uses the technically accepted Smoke05 source baseline with product identity/version changes and the separately approved TDLib loader delta. The unchanged legacy backend, bridge and selected audio behavior are preserved. Later unrelated waveform source changes were excluded from this isolated build without changing the working tree's files.

Release win-x64 self-contained publish and static runtime checks passed. Focused tests against the resulting managed assemblies passed: version/identity plus 17 inert TDLib dependency validation cases. ZIP inventory, hashes, clean defaults and extraction are checked separately. No new player/native execution or rendered UI acceptance has been performed. Clean-Windows behavior, SxS activation and dynamic DirectX selection remain NOT VERIFIED.

No personal UserData, library database, playlist, Telegram session or logs are included. The accepted configured appearance is retained as clean seeds. See INSTALL.md and THIRD_PARTY_NOTICES.md before future authorized use/distribution.
