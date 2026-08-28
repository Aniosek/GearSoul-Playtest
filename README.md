# GearSoul — Pre-Alpha Multiplayer Playtest

**GearSoul** to rozwijana w Unreal Engine gra o przetrwaniu, pracy, nauce zawodów i budowaniu własnej historii. Nie narzuca graczowi roli wojownika — postać może rozwijać się przez pracę, rzemiosło, handel, budowę oraz współpracę z innymi.

> To wczesna wersja techniczna. Grafika, interfejs, balans i zawartość nadal się zmieniają.

## Pobierz aktualną wersję

### [Pobierz GearSoul v0.2.3 Pre-Alpha Multiplayer (Windows)](https://github.com/Aniosek/GearSoul-Playtest/releases/download/v0.2.3/GearSoul_v0.2.3_PreAlpha_Multiplayer_Windows.zip)

Rozmiar archiwum: około **603 MiB**.

1. Pobierz i rozpakuj cały plik ZIP.
2. Nie uruchamiaj gry bezpośrednio z wnętrza archiwum.
3. Uruchom `START_GearSoul_Solo.bat`, `START_GearSoul_Host.bat` albo `START_GearSoul_Join.bat`.

Przy połączeniu przez Internet host musi dopuścić grę w Zaporze Windows i przekierować **UDP 7777**. Ta wersja używa listen-servera.

## Co zmieniło się w v0.2.3

- kolejne rudy, kamienie, glina i produkty stanowisk pojawiają się w wolnych miejscach zamiast jeden na drugim,
- bezpieczne rozmieszczanie fizycznych przedmiotów jest wykonywane przez serwer bez gwałtownych impulsów,
- przedmioty wczytane z zapisu zachowują swoją zapisaną pozycję,
- plac budowy wyjaśnia, że materiały można dostarczać pojedynczo i zachowuje postęp,
- palisada nadal wymaga łącznie 5 kłód i 5 cykli młotkiem, a fundament 4 kamieni i 6 cykli młotkiem.

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

Pełna lista znajduje się w pliku `CZYTAJ_TO_GearSoul_v0.2.3.md` wewnątrz paczki.

## Integralność pobrania

SHA-256:

```text
F056B266D3A00050B9732735AC26C29E3B91908902F07265B82D69C65D4AF425
```

## Status projektu

- **Wersja:** v0.2.3 Pre-Alpha Multiplayer Playtest
- **Platforma:** Windows 64-bit
- **Silnik:** Unreal Engine 5.8
- **Stan:** aktywny rozwój

Kod źródłowy gry nie jest publikowany w tym repozytorium. Zawartość wydania jest spakowana jako Unreal Pak/IoStore; nie da się jednak zagwarantować absolutnej niemożliwości analizy aplikacji uruchamianej na komputerze testera.

Copyright © 2026 Aniosek. Publiczna paczka służy do testowania i nie udziela praw do kodu ani zasobów projektu.
