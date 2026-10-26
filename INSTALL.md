# Portable installation

Status: private local candidate, not a published release. Runtime acceptance on a clean Windows host is NOT VERIFIED.

Intended platform: Windows x64 with the OS Universal CRT and graphics facilities required by the accepted application. The managed application targets Windows 10 build 19041 or later. Packaged .NET/WPF 10.0.11, x86 backend, VC runtime and DirectX helper DLLs do not require a separate installer. Compatibility with every Windows version, driver and audio device has not been established.

1. Verify the complete ZIP against its SHA256SUMS.txt, then extract it into a new writable directory.
2. Keep `runtime`, `Backend`, `Tools`, `profile` and notices beside the root executable.
3. Launch `foobar2000 Alienov edition.exe` when runtime testing or use is authorized.
4. Add your own music. The package contains no music library, playlists, account sessions or personal UserData. Telegram account setup requires the user's own credentials and network access; it does not download native components.

The clean profile keeps the accepted configured appearance. On first launch the player creates its portable `UserData` below the extracted root. Do not launch the internal backend or the Winamp compatibility sentinel directly. All processes owned by the player must finish before files are replaced.

For future updates, back up and preserve existing `UserData`; never replace it with another user's profile. Do not extract a new version over a running player. Automatic updating is not implemented by this task.
