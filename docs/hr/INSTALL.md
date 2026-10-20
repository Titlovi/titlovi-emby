# Instalacija Titlovi.com dodatka za Emby Server 4.10.x

[English](../../INSTALL.md) · [Hrvatski](INSTALL.md) · [Српски](../sr-Cyrl/INSTALL.md)

## Zahtjevi

- Emby Server **4.10.x**.
- Titlovi.com račun s API pristupom.
- Emby **DLL**, a ne Jellyfin ZIP ili GitHubova arhiva „Source code”.

## Instalacija / nadogradnja

1. Na stranici [Releases](https://github.com/Titlovi/titlovi-emby/releases) preuzmite `Emby.Titlovi.dll` i `SHA256SUMS.txt` iz najnovijeg kompatibilnog izdanja.
2. Provjerite SHA-256. U PowerShellu izvršite `Get-FileHash -Algorithm SHA256 .\Emby.Titlovi.dll` i usporedite rezultat s datotekom `SHA256SUMS.txt`.
3. Zaustavite Emby Server. Pri nadogradnji spremite stari DLL i konfiguraciju u **zasebnu mapu izvan aktivne mape dodataka**.
4. Pronađite **stvarnu mapu dodataka Emby Servera**. Putanja ovisi o instalaciji i postavkama podatkovne mape.
5. U nju kopirajte novi `Emby.Titlovi.dll`, zamjenjujući samo stari Titlovi DLL ako postoji. Dodatni Common/Core DLL nije potreban.
6. Pokrenite Emby i potvrdite da se **Titlovi.com** nalazi među instaliranim dodacima.
7. Konfigurirajte Titlovi.com račun i postavke. Pretražite i preuzmite titl za film ili epizodu.

## Povratak na stariju verziju i otklanjanje problema

Ako se dodatak ne učita, provjerite verziju Embyja, mapu dodataka i zapisnike. Za povratak zaustavite Emby, vratite kompatibilan prethodni DLL **i konfiguraciju**, ponovno ga pokrenite te testirajte pretragu. Ne mijenjajte druge dodatke.

**Poznato ograničenje Embyja 4.10:** nastavak naziva datoteke može odgovarati traženom jeziku čak i kada dodatak u rezultatima prikazuje stvarni jezik titla.

[Izvorni kod i podrška](https://github.com/Titlovi/titlovi-unified) · [Povratak na preuzimanje](README.md)
