# foobar2000 Alienov edition

**foobar2000 Alienov edition**

An unofficial, portable Windows audio player combining a modern x64 WPF interface with the classic foobar2000 0.9.6.9 x86 playback engine.

## ⬇ Download

<!-- ALIENOV-RELEASE:BEGIN -->
## Current portable release: beta 0.3.1

**[Download the complete Windows x64 portable ZIP](https://github.com/hawkedw/foobar2000-alienov-edition/releases/download/v0.3.1/foobar2000-Alienov-edition-beta-0.3.1-win-x64.zip)**

**GitHub Code > Download ZIP is NOT the portable distribution. Use the release asset above.**

- Size: 204241640 bytes.
- SHA-256: `22B0D5B58D303EF2E5C399A7BCE2934B435ABC2E6E5E42485C6B35B1C054FC8E`
- [Release notes](https://github.com/hawkedw/foobar2000-alienov-edition/releases/tag/v0.3.1)
- [SHA256SUMS.txt](https://github.com/hawkedw/foobar2000-alienov-edition/releases/download/v0.3.1/SHA256SUMS.txt)

Runtime/visual acceptance of this candidate: NOT VERIFIED. Existing profiles are preserved; fresh installs receive the configured factory UI. Third-party redistribution limitations remain disclosed in the notices and release notes.


<!-- ALIENOV-RELEASE:END -->

## Getting started

1. Download the portable ZIP using the link above.
2. Extract the archive into a folder of your choice, for example `C:\foobar2000 Alienov edition`.
3. Launch **foobar2000 Alienov edition.exe**.
4. Configure your music library and enjoy your music.

The portable package includes the required application runtime, legacy playback backend, visualization components and bundled dependencies.

No separate application installation is required.

## Features

- Modern, configurable WPF desktop interface.
- Classic foobar2000 0.9.6.9 playback engine.
- Local music library powered by SQLite.
- Playlist management and library navigation.
- Customizable layouts and themes.
- Integrated MilkDrop visualization.
- Portable user settings, library database and application state.
- Telegram integration.
- GitHub-based update checking through **Help → Check for Updates**.

## Portable storage

Application data is intended to remain inside the extracted portable directory, including:

- `profile/UserData/Local/Library/library.db` — SQLite music library.
- `profile/UserData/Local` — local settings, caches and application data.
- `profile/UserData/Roaming` — roaming-style application preferences and configuration.

The updater is designed to preserve user data and existing configurations when installing a newer version.

Music library paths may require adjustment when moving the player to another computer.

## Updates

To check for a newer version, open:

**Help → Check for Updates**

The player checks published GitHub Releases for compatible versions and offers a download when an update is available.

Downloading and installation require user confirmation. Automatic update checking can optionally be enabled in Preferences.

The integrated updater is a beta feature. Its complete real-world installation, rollback and restart workflow has not yet received end-to-end runtime acceptance.

## Release verification

The current portable ZIP checksum is shown in the Download section above and in [SHA256SUMS.txt](SHA256SUMS.txt).

## Beta status

This is an experimental beta release. Bugs, incomplete functionality and compatibility issues may occur.

Clean-Windows operation and the complete automatic-update lifecycle have not yet been independently verified.

Feedback and bug reports are welcome through [GitHub Issues](https://github.com/hawkedw/foobar2000-alienov-edition/issues).

## Documentation

- [Installation instructions](INSTALL.md)
- [Release notes](RELEASE_NOTES.md)
- [Known issues](KNOWN_ISSUES.md)
- [Changelog](CHANGELOG.md)
- [Licensing information](LICENSING.md)
- [Third-party notices](THIRD_PARTY_NOTICES.md)
- [Commercial licensing](COMMERCIAL-LICENSING.md)

## Licensing and third-party components

Original eligible project-owned materials are licensed under **PolyForm Noncommercial 1.0.0**.

This is a source-available licensing model, not an OSI-approved open-source license. The complete application source code is not currently published in this repository.

Third-party components remain subject to their respective licenses and copyright terms. Redistribution permissions and compliance obligations for certain bundled components have not yet been fully resolved.

**foobar2000 Alienov edition is an independent, unofficial project and is not affiliated with or endorsed by the original foobar2000 developers.**

---

**Project maintained by [hawkedw](https://github.com/hawkedw).**
