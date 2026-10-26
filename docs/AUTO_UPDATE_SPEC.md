# Future portable updater contract — specification only

Repository: `hawkedw/foobar2000-alienov-edition`. Current version: `0.3.0`. Channel: `beta`. Tag: `v0.3.0`. Next patch: `0.3.1`. Release title: `foobar2000 Alienov edition beta 0.3.0`. Complete Windows x64 asset: `foobar2000-Alienov-edition-beta-0.3.0-win-x64.zip`.

The private build's authoritative source is `app/ProductVersion.props`; `release.json` is generated metadata for this prepared repository. Internal assembly, IPC, profile and database identities remain stable. Backend version and bridge protocol are independent of the product version.

GitHub's pre-release flag and explicit channel define beta eligibility. The tag v0.3.0 has no SemVer prerelease suffix, so do not infer channel from the numeric version or use the latest-stable endpoint for beta discovery. Enumerate releases, exclude drafts and select only the user's channel and architecture; stable users must not silently receive beta.

Future implementation must validate metadata, expected asset name, size and trusted authenticity evidence before use. A checksum served beside an artifact detects corruption but is not an independent signature. Reject ZIP path traversal, duplicate/case-colliding entries and unexpected payload. Extract to a separate staging directory, verify every immutable file, and wait for Desktop plus its exact owned backend generation to shut down before replacement.

Preserve portable UserData, user settings, libraries, playlists, credentials and sessions. Never copy another user's profile or overwrite existing UserData with defaults. Seed defaults only through the existing first-run contract. Keep a recoverable previous program generation, use bounded replacement with clear failure handling, and do not scan personal music. The updater must not modify reference installations or the selected audio policy. No updater or download behavior is implemented by this document.
