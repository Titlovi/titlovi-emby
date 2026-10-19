# Installing Titlovi.com on Emby Server 4.10.x

> **Not yet released.** Official Unified `2.0.0.0` downloads are not currently available from this repository. These instructions describe the future **manual DLL** distribution process; they are not an instruction to install a preview binary.

## Supported host

The first official Unified release targets **Emby Server 4.10.x**. Compatibility with earlier or later Emby versions is not implied without testing. This is an Emby-specific DLL, **not** the Jellyfin plugin package.

## New installation — after publication

1. Open this repository's [Releases](https://github.com/Titlovi/titlovi-emby/releases) page and select the approved release compatible with Emby Server 4.10.x.
2. Download `Emby.Titlovi.dll` and its published SHA-256 checksum. Verify the file before installing. Use a DLL from an actual GitHub Release, **not** an Actions artifact, source checkout, or preview build.
3. Stop Emby Server.
4. Locate the active Emby Server **plugins directory** for that installation. Its exact filesystem path depends on the platform and Emby data-directory configuration; do not assume that the application installation folder is the plugins directory.
5. Copy `Emby.Titlovi.dll` to that plugins directory. Do **not** add a separate Common/Core assembly and do not copy Jellyfin ZIP contents.
6. Start Emby Server. Confirm that **Titlovi.com** appears among installed plugins.
7. Open the plugin's settings, enter your Titlovi.com account credentials, and save the configuration.
8. Test one subtitle search and download before considering installation successful.

A Titlovi.com account with the necessary API access is required.

## Updating an existing Emby plugin

Back up the existing plugin DLL and its configuration before updating. Stop Emby Server, replace **only the corresponding Titlovi plugin DLL** with the approved new release, then restart. Check the installed plugin identity, settings, and a real subtitle search/download. Do not delete unrelated plugin files or configurations.

## Known Emby 4.10 limitation

Emby Server 4.10.x has a known host limitation concerning alternative-language filename suffixes when a subtitle is saved. This limitation is accepted; the plugin preserves the **actual language reported by Titlovi.com** and does not implement a shared-logic filename workaround.

## Troubleshooting and rollback

If the plugin does not appear after restart, first verify the Emby Server version, the active plugins directory, and the server logs. If subtitle search fails, verify the Titlovi.com account/API access and plugin configuration.

For rollback, stop Emby Server, restore your backed-up compatible plugin DLL and configuration, then restart and re-test. A previous DLL is suitable for rollback only when compatible with the installed Emby host and the saved configuration. **Do not** use Jellyfin packages or manually modify another plugin's data.

## Source and release traceability

The complete, shared source code is maintained at [Titlovi/titlovi-unified](https://github.com/Titlovi/titlovi-unified). Every future official Emby release must point to the matching approved Unified source tag and provide verifiable checksums. See the [Unified installation documentation](https://github.com/Titlovi/titlovi-unified/blob/main/docs/en/INSTALL.md) for additional context.
