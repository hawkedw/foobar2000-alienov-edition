# foobar2000 Alienov edition beta 0.3.8

Complete Windows x64 portable prerelease. This release includes the accepted changes developed since public beta 0.3.5; private beta 0.3.6 and 0.3.7 were not public releases.

- Improve durable library indexing with generation checkpoints, interruption/resume, bounded retries and root progress.
- Improve CUE handling and classify unsupported or unresolved descriptors as nonfatal skips where appropriate.
- Keep completed Library roots quiet while providing accurate scan totals, warning categories and compact diagnostics.
- Add Save full diagnostic log to export all stored diagnostic records from one consistent generation/epoch, beyond the old diagnostics page limit, without starting a scan.
- Include the accepted Telegram connection/authorization workflow, source Refresh, history indexing and Search navigation improvements.
- Preserve existing settings, playlists and Telegram sessions through the accepted update path. Keep the integrated GitHub updater and its integrity/recovery protections.
- Include Library Tree Refresh/Analysis admission fixes, forced BPM feedback, package-root AcoustID/fpcalc resolution, keyboard context-menu ownership and status-message expiry protection.

## Updating and database rollback

The package includes the complete runtime, backend and updater. Existing profile/UserData is not replaced by the updater. Back up your portable installation before updating.

For users coming from beta 0.3.5, the first new Desktop initialization migrates the library database from schema 32 to 33. Beta 0.3.5 cannot reopen a schema-33 database. Before updating, close all database owners and retain a fresh SQLite-consistent backup of the complete library database and profile, paired with the old application. A live main-file-only copy can omit committed WAL data. Rollback requires restoring the compatible application and the complete matching database backup after stopping all owners; do not mix WAL/SHM files from different database generations. Program-file rollback alone is insufficient.

## Verification and limitations

Exact package inventory, CRC, SHA-256, manifests, privacy checks, frozen identities and trusted updater contracts passed. The updater contract binaries are unchanged from public beta 0.3.5. One controlled private 0.3.7 to 0.3.8 installation completed through the trusted helper, preserving user state. The installed compact diagnostics and complete 1218-record export were accepted; Telegram connection/source state and quiet Library status were retained without indexing.

Clean-Windows acceptance, native MilkDrop device-loss recovery on the previously affected machine, a full public 0.3.5 to 0.3.8 live installation/restart and untested failure paths remain NOT VERIFIED. Manual native Save-dialog Cancel acceptance remains NOT VERIFIED. This is not a claim that all graphics issues or all update/rollback scenarios are resolved.

The application is unsigned. SHA-256 and GitHub asset digests verify artifact integrity; they are not an independent publisher signature.

The exact accepted ZIP retains historical local-preparation status fields and documents. The owner's current authorization supersedes the earlier LOCAL MODE B publication hold for this release; the immutable archive has not been rebuilt or altered to change those fields.

## Licensing and redistribution

PolyForm Noncommercial and all existing third-party notices remain unchanged. Owner publication authorization does not grant third-party rights or certify licensing compliance. Existing redistribution, corresponding-source, attribution and notice limitations remain disclosed in THIRD_PARTY_NOTICES.md and LICENSING.md; this release makes no new legal-clearance claim.
