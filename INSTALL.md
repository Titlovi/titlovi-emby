# Installing Titlovi.com on Emby Server 4.10.x

[English](INSTALL.md) · [Hrvatski](docs/hr/INSTALL.md) · [Српски](docs/sr-Cyrl/INSTALL.md)

> **Not yet published.** Version 2.0.0.0 is being prepared; the following steps apply after an approved release becomes available.

## Requirements

- Emby Server **4.10.x**.
- A Titlovi.com account with API access.
- The Emby **DLL**, not the Jellyfin ZIP or GitHub's “Source code” archive.

## Installation / upgrade

1. On [Releases](https://github.com/Titlovi/titlovi-emby/releases), choose the latest compatible release and download `Emby.Titlovi.dll` plus `SHA256SUMS.txt`.
2. Verify the SHA-256 digest. In PowerShell run: `Get-FileHash -Algorithm SHA256 .\Emby.Titlovi.dll` and compare with `SHA256SUMS.txt`.
3. Stop Emby Server. If updating, back up the installed `Emby.Titlovi.dll` and its configuration in a **separate folder outside** the active plugins directory.
4. Find the **actual Emby plugins directory** for your server. Its location depends on your installation and data-directory settings; do not assume the application install directory is the same.
5. Copy the new `Emby.Titlovi.dll` into that plugins directory, replacing only the old Titlovi plugin DLL if present. Do not install an extra Common/Core DLL.
6. Start Emby and confirm **Titlovi.com** appears under installed plugins.
7. Configure your Titlovi.com credentials and preferences. Search for and download a subtitle for a film or episode.

## Rollback and troubleshooting

If the plugin fails to load, verify the server version, plugins path, and Emby logs. To roll back, stop Emby, restore the compatible backed-up DLL **and configuration**, restart, then repeat the search/download test. Do not modify unrelated plugins.

**Known Emby 4.10 limitation:** when alternative-language search is used, the saved filename may use the requested language suffix even though the plugin reports the subtitle's real language.

[Source code and support](https://github.com/Titlovi/titlovi-unified) · [Back to downloads](README.md)
