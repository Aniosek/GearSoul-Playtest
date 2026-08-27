# GearSoul — Pre-Alpha Multiplayer Playtest

**GearSoul** to rozwijana w Unreal Engine gra o przetrwaniu, pracy, nauce zawodów i budowaniu własnej historii. Nie narzuca roli wojownika — postać może poświęcić się rzemiosłu, wydobyciu, handlowi, logistyce albo życiu społeczności.

> To wczesny build techniczny. Testujemy mechaniki, multiplayer i stabilność, a nie końcową grafikę ani balans.

## Pobierz aktualną wersję

### [Pobierz GearSoul v0.2.0 Pre-Alpha Multiplayer Playtest (Windows)](https://github.com/Aniosek/GearSoul-Playtest/releases/download/v0.2.0/GearSoul_v0.2.0_PreAlpha_Multiplayer_Windows.zip)

- Rozmiar ZIP: około **597 MB**
- Platforma: Windows 64-bit
- Silnik: Unreal Engine 5.8
- SHA-256: `B484DFDF4057820FCEC1C9FE4F664A8C4F2C34B64CC1626108305A8D160AD89E`

Pełna paczka pozostaje w [GitHub Releases](https://github.com/Aniosek/GearSoul-Playtest/releases), ponieważ właśnie tam GitHub pokazuje liczbę pobrań pliku. Gałąź `main` zawiera instrukcje, checklistę i sumę kontrolną — bez kodu źródłowego gry.

## Jak uruchomić

1. Pobierz ZIP i rozpakuj **cały** folder.
2. Nie uruchamiaj gry bezpośrednio z archiwum.
3. Wybierz launcher:
   - `START_GearSoul_Solo.bat` — test solo,
   - `START_GearSoul_Host.bat` — host multiplayer,
   - `START_GearSoul_Join.bat` — dołączenie do hosta.

W sieci lokalnej klient wpisuje IPv4 hosta. Przy grze przez Internet host musi dopuścić aplikację w Zaporze Windows i przekierować **UDP 7777** na routerze. v0.2.0 używa listen-servera, więc host również jest graczem.

## Co nowego w v0.2.0

- publiczny test multiplayer z hostowaniem i dołączaniem po IP,
- mapa obejmująca systemy etapów 0–41,
- 41 fizycznych przedmiotów dostępnych do podnoszenia,
- lekki zestaw startowy: FireDrill, StonePickaxe i MasonryHammer,
- fizyczny plecak, masa, objętość i limity slotów,
- claimy, barter, wozy, drogi, karawany i regiony,
- pełne łańcuchy drewna, cegieł, metalurgii, rolnictwa i chleba,
- jakość, zużycie i naprawa narzędzi,
- krwawienie, infekcja i leczenie wykonywane przez drugiego gracza,
- kataklizmy środowiskowe i narzędzia testowe,
- stabilność sprawdzona lokalnie dla 2, 5, 10 i 15 klientów.

## Krótka checklista testera

- [ ] Host i klienci widzą te same postacie, przedmioty i zmiany świata.
- [ ] Podnoszenie i odkładanie nie blokuje postaci ani interakcji `E`.
- [ ] Przedmioty nie wystrzeliwują, nie wirują i nie wpadają pod mapę.
- [ ] Masa, objętość, sloty i plecak reagują na realną zawartość.
- [ ] Drzewo daje kłody, a kłody można przerobić na opał.
- [ ] Wydobycie kamienia, żelaza i węgla nie blokuje gracza po wyczerpaniu złoża.
- [ ] Budowanie i naprawa wymagają właściwych materiałów, narzędzi i uprawnień.
- [ ] Skrzynie, barter, wóz i karawana działają pomiędzy graczami.
- [ ] Drugi gracz może opatrzyć ranę i leczyć infekcję fizycznymi środkami.
- [ ] Dłuższa sesja nie powoduje utraty sterowania, crasha ani rozjazdu stanu.

Pełna lista znajduje się w [TESTING_CHECKLIST_PL.md](TESTING_CHECKLIST_PL.md).

## Komendy mapy testowej

Otwórz konsolę klawiszem `~`, wpisz `GSTestHelp` i zatwierdź Enterem. Przykłady:

```text
GSTestStatus
GSTestInventory
GSTestGo Resources
GSTestGo Trade
GSTestCataclysm Heatwave 10 0.75
GSTestCataclysm Storm 10 0.75
GSTestCataclysm Clear
```

## Zgłaszanie błędu

Napisz, czy grałeś solo, jako host czy klient, ilu było graczy, jakie kroki wykonałeś, czego oczekiwałeś i co stało się naprawdę. Dołącz screenshot/film oraz najnowszy log, jeśli możesz.

```text
%LOCALAPPDATA%\GearlSoul1\Saved\Logs
```

Pamiętaj, aby nie publikować swojego adresu IP ani innych prywatnych danych.

## Prawa i licencje

Kod źródłowy nie jest publikowany. Zawartość gry jest ugotowana i spakowana przez Unreal Pak/IoStore. Modele środowiska wykorzystane w prototypie pochodzą z Poly Haven na licencji CC0; zawartość Unreal jest częścią spakowanego produktu zgodnie z właściwą licencją Epic.

Copyright © 2026 Aniosek. Paczka służy do testowania i nie udziela praw do kodu ani zasobów projektu. Oprogramowanie oraz licencjonowana technologia i zawartość są udostępniane „tak jak są”, bez dodatkowych zapewnień i gwarancji.
