# Titlovi.com за Emby

[English](../../README.md) · [Hrvatski](../hr/README.md) · [Српски](README.md)

[![Emby Server](https://img.shields.io/badge/Emby%20Server-4.10.x-0076bb)](INSTALL.md)
[![.NET Standard](https://img.shields.io/badge/.NET%20Standard-2.0-512BD4)](https://github.com/Titlovi/titlovi-unified/blob/main/src/Emby/Emby.Titlovi.csproj)
[![Latest release](https://img.shields.io/github/v/release/Titlovi/titlovi-emby?label=release&color=0076bb)](https://github.com/Titlovi/titlovi-emby/releases/latest)
[![DLL downloads](https://img.shields.io/github/downloads/Titlovi/titlovi-emby/Emby.Titlovi.dll?label=DLL%20downloads&color=4c1)](https://github.com/Titlovi/titlovi-emby/releases)

**Претражујте и преузимајте титлове директно у Emby Server-у 4.10.x.**

**[⬇ Преузми најновије издање](https://github.com/Titlovi/titlovi-emby/releases/latest)** · [Упутство за инсталацију](INSTALL.md) · [Изворни код](https://github.com/Titlovi/titlovi-unified)

> **Статус до првог објављивања:** Званична верзија 2.0.0.0 још је у припреми и није доступна за преузимање. Ознаке верзије и броја преузимања аутоматски ће приказивати податке после објављивања.

## Преузимање

Отворите **[GitHub Releases](https://github.com/Titlovi/titlovi-emby/releases)** и преузмите **`Emby.Titlovi.dll`** из најновијег компатибилног издања. За проверу преузетог DLL-а служи **`SHA256SUMS.txt`**.

**Немојте користити GitHub-ове аутоматски направљене архиве „Source code (zip/tar.gz)” као инсталациони пакет.** Изворни код налази се у [Titlovi/titlovi-unified](https://github.com/Titlovi/titlovi-unified).

## Кратко упутство за инсталацију

1. Зауставите Emby Server. При надоградњи сачувајте резервну копију постојећег Titlovi DLL-а и конфигурације.
2. Копирајте `Emby.Titlovi.dll` у **активну фасциклу додатака Emby Server-а**.
3. Поново покрените Emby и проверите да ли се **Titlovi.com** приказује међу инсталираним додацима.
4. Унесите податке свог Titlovi.com налога, па претражите и преузмите титл.

Прочитајте [детаљно упутство за инсталацију, надоградњу и повратак на претходну верзију](INSTALL.md).

## Могућности

- Претрага титлова за филмове и епизоде серија на Titlovi.com.
- Опционо укључивање алтернативних титлова на српском, хрватском и босанском језику.
- Рангирање по називу издања видеа, без искључивања иначе ваљаних резултата.
- Обрада ZIP архива сезона и целих серија, угнежђених архива и више епизода.
- Подршка за формате SRT, SUB, TXT, SSA и ASS.
- Опционо претварање преузетих титлова у UTF-8 и детаљно бележење рада.

Резултати приказују стварни језик титла и не спајају различите Titlovi медијске ID-ове.

## Захтеви и позната ограничења

- **Emby Server 4.10.x**; компатибилност са другим верзијама није потврђена.
- Titlovi.com налог са потребним API приступом.
- **Само ручна инсталација** — нема Emby каталога додатака ни аутоматског ажурирања.
- **Познато ограничење Embyја 4.10:** када се тражи алтернативни језик, језички суфикс сачуваног титла може одговарати језику претраге, а не стварном језику. Резултати претраге и даље приказују стварни језик титла.

## Изворни код, подршка и лиценца

Овај репозиторијум служи **само за преузимање Emby додатка**. Изворни код, пријаве проблема, развој и лиценца налазе се на [Titlovi/titlovi-unified](https://github.com/Titlovi/titlovi-unified). **Jellyfin пакети се не могу инсталирати у Emby.**

Лиценца је GPL-3.0. Првобитни рад Матка на Titlovi.com/Jellyfin додатку наведен је у заједничком репозиторијуму.
