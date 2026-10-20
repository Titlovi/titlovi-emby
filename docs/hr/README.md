# Titlovi.com za Emby

[English](../../README.md) · [Hrvatski](README.md) · [Српски](../sr-Cyrl/README.md)

[![Emby Server](https://img.shields.io/badge/Emby%20Server-4.10.x-0076bb)](INSTALL.md)
[![.NET Standard](https://img.shields.io/badge/.NET%20Standard-2.0-512BD4)](https://github.com/Titlovi/titlovi-unified/blob/main/src/Emby/Emby.Titlovi.csproj)
[![Latest release](https://img.shields.io/github/v/release/Titlovi/titlovi-emby?label=release&color=0076bb)](https://github.com/Titlovi/titlovi-emby/releases/latest)
[![DLL downloads](https://img.shields.io/github/downloads/Titlovi/titlovi-emby/latest/Emby.Titlovi.dll?label=DLL%20downloads%20(latest)&color=4c1)](https://github.com/Titlovi/titlovi-emby/releases)

**Pretražujte i preuzimajte titlove izravno u Emby Serveru 4.10.x.**

**[⬇ Preuzmi najnovije izdanje](https://github.com/Titlovi/titlovi-emby/releases/latest)** · [Upute za instalaciju](INSTALL.md) · [Izvorni kod](https://github.com/Titlovi/titlovi-unified)

> **Status do prve objave:** Službena verzija 2.0.0.0 još je u pripremi i nije dostupna za preuzimanje. Oznake izdanja i preuzimanja automatski će prikazivati podatke nakon objave.

## Preuzimanje

Otvorite **[GitHub Releases](https://github.com/Titlovi/titlovi-emby/releases)** i preuzmite **`Emby.Titlovi.dll`** iz najnovijeg kompatibilnog izdanja. Datoteka **`SHA256SUMS.txt`** omogućuje provjeru preuzetog DLL-a.

**Nemojte instalirati GitHubove automatski generirane arhive „Source code (zip/tar.gz)”.** Izvorni kod nalazi se u [Titlovi/titlovi-unified](https://github.com/Titlovi/titlovi-unified).

## Ukratko o instalaciji

1. Zaustavite Emby Server. Pri nadogradnji izradite sigurnosnu kopiju postojećeg Titlovi DLL-a i konfiguracije.
2. Kopirajte `Emby.Titlovi.dll` u **aktivnu mapu dodataka Emby Servera**.
3. Ponovno pokrenite Emby i provjerite nalazi li se **Titlovi.com** među instaliranim dodacima.
4. Unesite podatke svojeg Titlovi.com računa, a zatim pretražite i preuzmite titl.

Pročitajte [detaljne upute za instalaciju, nadogradnju i povratak na stariju verziju](INSTALL.md).

## Mogućnosti

- Pretraživanje titlova za filmove i epizode serija na Titlovi.com.
- Neobavezno uključivanje titlova na srpskom, hrvatskom i bosanskom jeziku kao alternativnih rezultata.
- Rangiranje podudarnosti s izdanjem videozapisa bez isključivanja valjanih rezultata.
- Obrada ZIP arhiva cijelih sezona ili serija, ugniježđenih arhiva i više epizoda.
- Podrška za formate SRT, SUB, TXT, SSA i ASS.
- Neobavezna pretvorba preuzetih titlova u UTF-8 i detaljno bilježenje rada.

Rezultati prikazuju stvarni jezik titla i ne spajaju različite Titlovi medijske ID-ove.

## Zahtjevi i poznata ograničenja

- **Emby Server 4.10.x**; druge verzije nisu potvrđene.
- Titlovi.com račun s potrebnim pristupom API-ju.
- **Ručna instalacija** — nema Emby kataloga dodataka ni automatskog ažuriranja.
- **Poznato ograničenje Embyja 4.10:** pri pretraživanju alternativnog jezika nastavak naziva spremljene datoteke može odgovarati traženom jeziku, a ne stvarnom jeziku titla. Rezultati pretrage i dalje navode stvarni jezik.

## Izvorni kod, podrška i licencija

Ovaj repozitorij služi **samo za preuzimanje Emby dodatka**. Izvorni kod, prijave problema, razvoj i informacije o licenciji nalaze se na [Titlovi/titlovi-unified](https://github.com/Titlovi/titlovi-unified). **Jellyfin paketi nisu namijenjeni Embyju.**

Licencija je GPL-3.0. Izvorni doprinos Matka projektu Titlovi.com/Jellyfin naveden je u zajedničkom repozitoriju.
