# GearSoul — Pre-Alpha Multiplayer Playtest

**GearSoul** to rozwijana w Unreal Engine gra o przetrwaniu, pracy, nauce zawodów i budowaniu własnej historii. Nie narzuca graczowi roli wojownika — postać może rozwijać się przez pracę, rzemiosło, handel, budowę oraz współpracę z innymi.

> To wczesna wersja techniczna. Grafika, interfejs, balans i zawartość nadal się zmieniają.

## Pobierz aktualną wersję

### [Pobierz GearSoul v0.3.0 Pre-Alpha Multiplayer (Windows)](https://github.com/Aniosek/GearSoul-Playtest/releases/download/v0.3.0/GearSoul_v0.3.0_PreAlpha_Multiplayer_Windows.zip)

Rozmiar archiwum: około **596 MiB**.

1. Pobierz i rozpakuj cały plik ZIP.
2. Nie uruchamiaj gry bezpośrednio z wnętrza archiwum.
3. Uruchom `START_GearSoul_Solo.bat`, `START_GearSoul_Host.bat` albo `START_GearSoul_Join.bat`.

Przy połączeniu przez Internet host musi dopuścić grę w Zaporze Windows i przekierować **UDP 7777**. Ta wersja używa listen-servera.

## Co zmieniło się w v0.3.0

- woda ma jakość, oczyszczanie opałem i fizyczną beczkę,
- mapa zawiera stado jeleni oraz woła z głodem, pragnieniem, zdrowiem i wytrzymałością,
- wół ciągnie wóz tylko podczas prowadzenia przez prawdziwego gracza,
- fauna może dawać ograniczone, fizyczne porcje surowego mięsa,
- osada wymaga 1 zestawu sztandaru, 4 kłód i 4 kamieni dostarczanych osobno,
- usługi osady istnieją tylko dzięki realnej wodzie, magazynowi, barterowi i stanowisku naprawczemu graczy.

## Najważniejsze testy

- hostowanie i dołączanie dwóch lub większej liczby graczy,
- wspólne podnoszenie, przenoszenie i używanie fizycznych przedmiotów,
- masa, objętość, sloty oraz działanie plecaka,
- barter, pojemniki, wóz, budowanie i uprawnienia claimu,
- wydobycie, ścinanie drzew, produkcja, ognisko, rolnictwo i medycyna,
- synchronizacja dnia, nocy, przetrwania oraz zdarzeń środowiskowych,
- wygląd i położenie siekiery, kilofa i młotka w prawej dłoni innych graczy.
- współdzielony postęp dostarczania materiałów i pracy na placu budowy.
- stabilne rozmieszczanie nowych surowców bez nakładania i wystrzeliwania obiektów.
- jakość, oczyszczanie i magazynowanie fizycznej wody.
- ruch stada, karmienie, pojenie i prowadzenie wołu z wozem.
- wspólne zakładanie osady oraz rejestrowanie istniejącej infrastruktury.

Pełna lista znajduje się w pliku `CZYTAJ_TO_GearSoul_v0.3.0.md` wewnątrz paczki.

## Integralność pobrania

SHA-256:

```text
D610E7AABD0DEC4ABF73C73AF2CCB6DEA558D1B2B62E232DAD82766ACEC68E6B
```

## Status projektu

- **Wersja:** v0.3.0 Pre-Alpha Multiplayer Playtest
- **Platforma:** Windows 64-bit
- **Silnik:** Unreal Engine 5.8
- **Stan:** aktywny rozwój

Kod źródłowy gry nie jest publikowany w tym repozytorium. Zawartość wydania jest spakowana jako Unreal Pak/IoStore; nie da się jednak zagwarantować absolutnej niemożliwości analizy aplikacji uruchamianej na komputerze testera.

Copyright © 2026 Aniosek. Publiczna paczka służy do testowania i nie udziela praw do kodu ani zasobów projektu.
