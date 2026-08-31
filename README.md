# GearSoul — Pre-Alpha Multiplayer Playtest

**GearSoul** to rozwijana w Unreal Engine gra o przetrwaniu, pracy, nauce zawodów i budowaniu własnej historii. Nie narzuca graczowi roli wojownika — postać może rozwijać się przez pracę, rzemiosło, handel, budowę oraz współpracę z innymi.

> To wczesna wersja techniczna. Grafika, interfejs, balans i zawartość nadal się zmieniają.

**Główna idea:** świat działa dlatego, że tworzą go gracze. Zobacz [wizję GearSoul](GEARSOUL_VISION.md) oraz [publiczną roadmapę](ROADMAP.md).

## Pobierz aktualną wersję

### [Pobierz GearSoul v0.6.0 Pre-Alpha Multiplayer (Windows)](https://github.com/Aniosek/GearSoul-Playtest/releases/download/v0.6.0/GearSoul_v0.6.0_PreAlpha_Multiplayer_Windows.zip)

Rozmiar archiwum: około **628 MiB**.

1. Pobierz i rozpakuj cały plik ZIP.
2. Nie uruchamiaj gry bezpośrednio z wnętrza archiwum.
3. Uruchom `START_GearSoul_Solo.bat`, `START_GearSoul_Host.bat` albo `START_GearSoul_Join.bat`.

Przy połączeniu przez Internet host musi dopuścić grę w Zaporze Windows i przekierować **UDP 7777**. Ta wersja używa listen-servera.

## GearSoul na screenach

![Kompaktowa mapa bez przenikalnego pierścienia wzgórz](screenshots/v0.4.1/01_kompaktowa_mapa_bez_przenikalnych_wzgorz.png)

Pozostałe screeny przedstawiają systemy obecne również w v0.4.1:

![Mapa testowa, transport i rzeka](screenshots/v0.4.0/01_mapa_i_transport.png)

![Las, rzeka i fizyczne surowce](screenshots/v0.4.0/02_las_rzeka_i_surowce.png)

![Przeskalowany polski ekwipunek](screenshots/v0.4.0/03_ekwipunek.png)

## Co zmieniło się w v0.6.0

- dodano fizyczną **Tablicę Zleceń Graczy** bez zadań generowanych przez NPC,
- zleceniodawca blokuje trzy prawdziwe srebrne monety, a drugi gracz przyjmuje pracę i dostarcza dwie kłody pojedynczo,
- ostatnia dostawa atomowo wypłaca nagrodę, a materiały trafiają do fizycznego magazynu odbioru,
- zlecenie, częściowe dostawy oraz oba magazyny escrow są trwale zapisywane i odporne na restart,
- ukończona praca pokazuje krótki polski komunikat XP nad właściwą postacią,
- prowadzenie wołu nie rozprzęga wozu, a ruch stad jest płynniejszy,
- dodano Punkty Wiedzy, działkę osady oraz kooperacyjną budowę domu i kuźni z prawdziwych materiałów.

Wcześniejsze systemy pozostają dostępne:

- mapa testowa ma naturalny teren, rzekę, las i lekkie stylizowane drzewa,
- ekwipunek otrzymał czytelny układ i prawidłowe skalowanie w 1600×900,
- las pamięta wycinkę, stan gleby, erozję i fizyczne sadzonki,
- most wymaga ośmiu osobnych kłód oraz pracy młotkiem i reaguje na przeciążony wóz,
- kuźnia wytwarza i naprawia żelazny kilof, siekierę oraz młotek z prawdziwych części,
- trzy regiony mają różne warunki magazynowania oraz fizyczne psucie żywności,
- nowe wizualizacje jedzenia i narzędzi pozostają lekkie dla multiplayera.

## Najważniejsze testy

- hostowanie i dołączanie dwóch lub większej liczby graczy,
- wspólne podnoszenie, przenoszenie i używanie fizycznych przedmiotów,
- masa, objętość, sloty oraz działanie plecaka,
- barter, pojemniki, wóz, budowanie i uprawnienia claimu,
- wydobycie, ścinanie drzew, produkcja, ognisko, rolnictwo i medycyna,
- synchronizacja dnia, nocy, przetrwania oraz zdarzeń środowiskowych,
- wygląd i położenie siekiery, kilofa i młotka w prawej dłoni innych graczy,
- wspólny postęp dostarczania materiałów i pracy na placu budowy,
- stabilne rozmieszczanie surowców bez nakładania i wystrzeliwania obiektów,
- oczyszczanie i magazynowanie fizycznej wody,
- ruch stada, karmienie, pojenie i prowadzenie wołu z wozem,
- odnowa lasu, budowa mostu, kowalstwo i regionalne magazyny żywności.
- Punkty Wiedzy, specjalizacje, pierścień działki oraz wspólna budowa domu i kuźni.
- Tablica Zleceń: utworzenie zlecenia, przyjęcie go przez drugiego gracza, dwie osobne dostawy, wypłata i odbiór materiałów.

Pełna lista znajduje się w `README_PL.md` wewnątrz paczki oraz w [checkliście testera](TESTING_CHECKLIST_PL.md).

## Zgłaszanie błędów

Błędy możesz zgłaszać przez **[formularz GitHub Issues](https://github.com/Aniosek/GearSoul-Playtest/issues/new?template=bug_report.yml)** albo wysłać na **[gearsoul00@gmail.com](mailto:gearsoul00@gmail.com)**.

W paczce gry znajduje się `CREATE_BUG_REPORT_PACKAGE.bat`, który zbiera dostępne logi, raporty awarii i zapis do jednego ZIP-a. Przejrzyj archiwum przed wysłaniem, a następnie przeciągnij je do formularza razem ze screenem lub filmem. Nie publikuj adresu IP ani danych konta.

## Dokumentacja publiczna

- [Wizja projektu](GEARSOUL_VISION.md)
- [Roadmapa](ROADMAP.md)
- [Changelog](CHANGELOG.md)
- [Licencje i zasoby prototypowe](LICENSES_AND_ASSETS.md)
- [Dziennik rozwoju](DEVELOPMENT_LOG.md)
- [Checklista testera](TESTING_CHECKLIST_PL.md)

## Integralność pobrania

SHA-256:

```text
7236114F0F1575BA86E6869656ADBABDB1488066134562D0F7975BC84B6F26B5
```

## Status projektu

- **Wersja:** v0.6.0 Pre-Alpha Multiplayer Playtest
- **Platforma:** Windows 64-bit
- **Silnik:** Unreal Engine 5.8
- **Stan:** aktywny rozwój

Kod źródłowy gry nie jest publikowany w tym repozytorium. Zawartość wydania jest spakowana jako Unreal Pak/IoStore; nie da się jednak zagwarantować absolutnej niemożliwości analizy aplikacji uruchamianej na komputerze testera.

Copyright © 2026 Aniosek — kod i autorska zawartość GearSoul. Publiczna paczka służy do testowania i nie udziela praw do kodu ani autorskich zasobów projektu. Informacje o wykorzystanych zasobach CC0 znajdują się wewnątrz paczki.
