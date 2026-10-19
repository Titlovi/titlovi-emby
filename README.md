# Titlovi.com for Emby

Official distribution repository for the **Titlovi.com** subtitle plugin for **Emby Server 4.10.x**.

**Release status: preparation only.** The first Unified **2.0.0.0** Emby release has **not been published**. There is currently no official `Emby.Titlovi.dll` download in this repository. Do not install development or preview artifacts as official releases.

## About this repository

The plugin is developed from one shared source tree for Emby and Jellyfin:

**[Titlovi/titlovi-unified](https://github.com/Titlovi/titlovi-unified)** — canonical source code, issues concerning the unified implementation, regression tests, documentation, and build instructions.

This repository is **Emby distribution only**. After a release is approved, its [GitHub Releases](https://github.com/Titlovi/titlovi-emby/releases) will provide:

- `Emby.Titlovi.dll` — the self-contained Emby plugin assembly (no separate Common/Core DLL);
- checksums for download verification;
- release notes and a link to the matching source tag in `titlovi-unified`.

**Emby installation is manual.** This project does not provide an Emby third-party plugin catalogue or an automatic-update feed.

The sibling [Titlovi Jellyfin distribution](https://github.com/Titlovi/titlovi-jellyfin) retains the original Jellyfin plugin catalogue and historic releases; its ZIP packages must **not** be installed on Emby.

## Installation

See [INSTALL.md](INSTALL.md) for the supported host, manual DLL installation steps, upgrading, and rollback. The instructions for downloading a release apply **only once an approved release is available**.

## Requirements

- Emby Server **4.10.x**.
- An active Titlovi.com account with API access, subject to Titlovi.com's terms.

## Licensing and provenance

Source code and attribution: [Titlovi Unified repository](https://github.com/Titlovi/titlovi-unified), including [LICENSE](https://github.com/Titlovi/titlovi-unified/blob/main/LICENSE) and [NOTICE.txt](https://github.com/Titlovi/titlovi-unified/blob/main/NOTICE.txt).

No binary from this repository should be redistributed as an official release before the maintainers have approved the corresponding Unified source, package and checksums.
