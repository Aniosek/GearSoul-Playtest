# GearSoul — Pre-Alpha Multiplayer Playtest

**GearSoul** to rozwijana w Unreal Engine gra o przetrwaniu, pracy, nauce zawodów i budowaniu własnej historii. Nie narzuca graczowi roli wojownika — postać może rozwijać się przez pracę, rzemiosło, handel, budowę oraz współpracę z innymi.

> To wczesna wersja techniczna. Grafika, interfejs, balans i zawartość nadal się zmieniają.

## Pobierz aktualną wersję

### [Pobierz GearSoul v0.2.1 Pre-Alpha Multiplayer (Windows)](https://github.com/Aniosek/GearSoul-Playtest/releases/download/v0.2.1/GearSoul_v0.2.1_PreAlpha_Multiplayer_Windows.zip)

Rozmiar archiwum: około **607 MiB**.

1. Pobierz i rozpakuj cały plik ZIP.
2. Nie uruchamiaj gry bezpośrednio z wnętrza archiwum.
3. Uruchom `START_GearSoul_Solo.bat`, `START_GearSoul_Host.bat` albo `START_GearSoul_Join.bat`.

Przy połączeniu przez Internet host musi dopuścić grę w Zaporze Windows i przekierować **UDP 7777**. Ta wersja używa listen-servera.

## Co zmieniło się w v0.2.1

- naprawiono blokadę sterowania po anulowaniu lub zamknięciu barteru,
- pierwszy oczekujący gracz może przygotować własną ofertę barterową,
- dodano używanie, wyposażanie i odkładanie przedmiotów z ekwipunku,
- narzędzia i przedmioty medyczne są widoczne w dłoni i replikowane w multiplayerze,
- dodano zoptymalizowane modele siekiery, młotka i kilofa po audycie geometrii, tekstur, pivotów i kolizji.

## Najważniejsze testy

- hostowanie i dołączanie dwóch lub większej liczby graczy,
- wspólne podnoszenie, przenoszenie i używanie fizycznych przedmiotów,
- masa, objętość, sloty oraz działanie plecaka,
- barter, pojemniki, wóz, budowanie i uprawnienia claimu,
- wydobycie, ścinanie drzew, produkcja, ognisko, rolnictwo i medycyna,
- synchronizacja dnia, nocy, przetrwania oraz zdarzeń środowiskowych,
- wygląd i położenie siekiery, kilofa i młotka w prawej dłoni innych graczy.

Pełna lista znajduje się w pliku `CZYTAJ_TO_GearSoul_v0.2.1.md` wewnątrz paczki.

## Integralność pobrania

SHA-256:

```text
0461CB543DED3AD3E8BD736EA1129162A0577F313772AF5480BB3AC44C2AB1D8
```

## Status projektu

- **Wersja:** v0.2.1 Pre-Alpha Multiplayer Playtest
- **Platforma:** Windows 64-bit
- **Silnik:** Unreal Engine 5.8
- **Stan:** aktywny rozwój

Kod źródłowy gry nie jest publikowany w tym repozytorium. Zawartość wydania jest spakowana jako Unreal Pak/IoStore; nie da się jednak zagwarantować absolutnej niemożliwości analizy aplikacji uruchamianej na komputerze testera.

Copyright © 2026 Aniosek. Publiczna paczka służy do testowania i nie udziela praw do kodu ani zasobów projektu.
