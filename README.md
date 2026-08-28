# GearSoul — Pre-Alpha Multiplayer Playtest

**GearSoul** to rozwijana w Unreal Engine gra o przetrwaniu, pracy, nauce zawodów i budowaniu własnej historii. Nie narzuca graczowi roli wojownika — postać może rozwijać się przez pracę, rzemiosło, handel, budowę oraz współpracę z innymi.

> To wczesna wersja techniczna. Grafika, interfejs, balans i zawartość nadal się zmieniają.

## Pobierz aktualną wersję

### [Pobierz GearSoul v0.2.2 Pre-Alpha Multiplayer (Windows)](https://github.com/Aniosek/GearSoul-Playtest/releases/download/v0.2.2/GearSoul_v0.2.2_PreAlpha_Multiplayer_Windows.zip)

Rozmiar archiwum: około **603 MiB**.

1. Pobierz i rozpakuj cały plik ZIP.
2. Nie uruchamiaj gry bezpośrednio z wnętrza archiwum.
3. Uruchom `START_GearSoul_Solo.bat`, `START_GearSoul_Host.bat` albo `START_GearSoul_Join.bat`.

Przy połączeniu przez Internet host musi dopuścić grę w Zaporze Windows i przekierować **UDP 7777**. Ta wersja używa listen-servera.

## Co zmieniło się w v0.2.2

- ścinanie, kopanie i wydobycie sprawdzają narzędzie, energię, durability oraz cooldown po stronie serwera,
- ruch używanego narzędzia jest replikowany i widoczny dla pozostałych graczy,
- palisada wymaga dostarczenia 5 osobnych kłód i wykonania 5 cykli młotkiem,
- fundament wymaga dostarczenia 4 kamieni i wykonania 6 cykli młotkiem,
- kilku uprawnionych graczy może wspólnie pracować przy jednym placu budowy,
- uszkodzone konstrukcje można naprawiać fizycznym materiałem i pracą młotka.

## Najważniejsze testy

- hostowanie i dołączanie dwóch lub większej liczby graczy,
- wspólne podnoszenie, przenoszenie i używanie fizycznych przedmiotów,
- masa, objętość, sloty oraz działanie plecaka,
- barter, pojemniki, wóz, budowanie i uprawnienia claimu,
- wydobycie, ścinanie drzew, produkcja, ognisko, rolnictwo i medycyna,
- synchronizacja dnia, nocy, przetrwania oraz zdarzeń środowiskowych,
- wygląd i położenie siekiery, kilofa i młotka w prawej dłoni innych graczy.
- współdzielony postęp dostarczania materiałów i pracy na placu budowy.

Pełna lista znajduje się w pliku `CZYTAJ_TO_GearSoul_v0.2.2.md` wewnątrz paczki.

## Integralność pobrania

SHA-256:

```text
71048A59A670122CD04BD40165999D93E8F969317952BF2FB5AF2AABE5F6CE47
```

## Status projektu

- **Wersja:** v0.2.2 Pre-Alpha Multiplayer Playtest
- **Platforma:** Windows 64-bit
- **Silnik:** Unreal Engine 5.8
- **Stan:** aktywny rozwój

Kod źródłowy gry nie jest publikowany w tym repozytorium. Zawartość wydania jest spakowana jako Unreal Pak/IoStore; nie da się jednak zagwarantować absolutnej niemożliwości analizy aplikacji uruchamianej na komputerze testera.

Copyright © 2026 Aniosek. Publiczna paczka służy do testowania i nie udziela praw do kodu ani zasobów projektu.
