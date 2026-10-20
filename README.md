# Titlovi.com for Emby

[English](README.md) · [Hrvatski](docs/hr/README.md) · [Српски](docs/sr-Cyrl/README.md)

[![Emby Server](https://img.shields.io/badge/Emby%20Server-4.10.x-0076bb)](INSTALL.md)
[![.NET Standard](https://img.shields.io/badge/.NET%20Standard-2.0-512BD4)](https://github.com/Titlovi/titlovi-unified/blob/main/src/Emby/Emby.Titlovi.csproj)
[![Latest release](https://img.shields.io/github/v/release/Titlovi/titlovi-emby?label=release&color=0076bb)](https://github.com/Titlovi/titlovi-emby/releases/latest)
[![DLL downloads](https://img.shields.io/github/downloads/Titlovi/titlovi-emby/latest/Emby.Titlovi.dll?label=DLL%20downloads%20(latest)&color=4c1)](https://github.com/Titlovi/titlovi-emby/releases)

**Search and download subtitles directly in Emby Server 4.10.x.**

**[⬇ Download latest release](https://github.com/Titlovi/titlovi-emby/releases/latest)** · [Installation guide](INSTALL.md) · [Source code](https://github.com/Titlovi/titlovi-unified)

> **Status (until first publication):** Official version 2.0.0.0 is being prepared and is not yet available to download. Release/download badges will become active after publication.

## Download

Open **[GitHub Releases](https://github.com/Titlovi/titlovi-emby/releases)** and download **`Emby.Titlovi.dll`** from the latest compatible release. You can also download **`SHA256SUMS.txt`** to verify the file.

**Do not use GitHub's automatically generated “Source code (zip/tar.gz)” archives as the plugin installer.** Source code is maintained in [Titlovi/titlovi-unified](https://github.com/Titlovi/titlovi-unified).

## Installation in brief

1. Stop Emby Server. If updating, back up the existing Titlovi DLL and configuration.
2. Copy `Emby.Titlovi.dll` to the **active Emby plugins directory**.
3. Restart Emby and confirm **Titlovi.com** appears in installed plugins.
4. Configure your Titlovi.com account, then search for and download a subtitle.

Read the [full installation, update, and rollback guide](INSTALL.md).

## Features

- Search for subtitles for movies and TV episodes on Titlovi.com.
- Optionally include Serbian, Croatian, and Bosnian alternative-language results.
- Rank release-name matches without excluding otherwise valid subtitles.
- Support season/series ZIP archives, nested archives, and grouped episodes.
- Download SRT, SUB, TXT, SSA, and ASS subtitle formats.
- Optionally convert downloaded subtitles to UTF-8 and enable diagnostic logging.

Search results preserve the actual subtitle language and keep different Titlovi media IDs distinct.

## Requirements and known limitations

- **Emby Server 4.10.x**; compatibility with other server versions has not been confirmed.
- A Titlovi.com account with the required API access.
- **Manual installation only** — no Emby plugin repository or automatic-update feed.
- **Known Emby 4.10 limitation:** for alternative-language searches, the saved subtitle filename suffix may use the requested language rather than the actual returned language. The plugin still identifies the correct language in search results.

## Source, support, and license

This repository is **only for Emby downloads**. Source code, bug reports, development, and licensing information are in [Titlovi/titlovi-unified](https://github.com/Titlovi/titlovi-unified). **Jellyfin packages cannot be installed in Emby.**

Licensed under GPL-3.0. Original Titlovi.com/Jellyfin work by Matko is acknowledged in the Unified repository.
