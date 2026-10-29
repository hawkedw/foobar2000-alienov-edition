# foobar2000 Alienov edition beta 0.3.1

- Fresh factory defaults now reproduce the saved daily-driver layout and appearance.
- Playlist columns, widths, formatting, grouping, colors and panel proportions are included in clean-install defaults.
- Existing user profiles remain preserved during upgrades; this release does not silently reset personalized UI.
- The GitHub updater, explicit installation consent and rollback support remain included.
- Portable ZIP entries use canonical forward slashes; package extraction and the 0.3.0 to 0.3.1 transition pass the actual published 0.3.0 updater contract without changing updater code or payload files.

## Download

Use the complete portable release asset, not GitHub Code > Download ZIP.

Asset: `foobar2000-Alienov-edition-beta-0.3.1-win-x64.zip`

Size: 204241640 bytes.

SHA-256: `22B0D5B58D303EF2E5C399A7BCE2934B435ABC2E6E5E42485C6B35B1C054FC8E`

## Known limitations

Actual visual/first-launch/end-to-end runtime acceptance of this candidate is **NOT VERIFIED**. Configuration, bootstrap, package hashes and synthetic tests have passed; those checks do not replace real player acceptance. Library Tree preserves the Ubuntu Light font preference; its availability and DPI-dependent appearance on other Windows systems are not verified.

The corrected archive passes path, complete extraction/hash and manifest-transition validation through the updater assemblies from published beta 0.3.0 and this beta 0.3.1. All payload files, native identities and factory UI defaults are unchanged. This focused compatibility check does not establish live GitHub download, shutdown, replacement, rollback or restart acceptance.

## Licensing and redistribution

The project-owned noncommercial license and all third-party notices remain unchanged. Noncommercial intent and owner approval do not confer third-party redistribution rights. Existing unresolved distribution/source/notice obligations include the extracted legacy foobar2000 backend, WilB-derived material, custom SACD components, Shpeck, Winamp/MilkDrop/presets, Microsoft VC/DirectX components, and FFmpeg/Chromaprint/transitive dependencies. This release note does not represent those restrictions as resolved. See LICENSING.md, DISTRIBUTION.md and THIRD_PARTY_NOTICES.md.
