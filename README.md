# GearSoul — Pre-Alpha Playtest

**GearSoul** to rozwijana w Unreal Engine gra o przetrwaniu, pracy, nauce zawodów i budowaniu własnej historii — bez narzuconej roli bohatera nastawionego wyłącznie na walkę.

> To wczesna wersja testowa. Jej zadaniem jest sprawdzenie podstawowych systemów, wygody sterowania i kierunku dalszego rozwoju.

## Pobierz aktualną wersję

### [Pobierz GearSoul v0.1.0 Pre-Alpha Playtest (Windows)](https://github.com/Aniosek/GearSoul-Playtest/releases/download/v0.1.0-prealpha-playtest/GearSoul_v0.1.0_PreAlpha_Playtest.zip)

Rozmiar archiwum: około **592 MB**.

1. Pobierz archiwum ZIP.
2. Rozpakuj cały folder w wybrane miejsce.
3. Uruchom plik `GearlSoul1.exe`.

Nie uruchamiaj gry bezpośrednio z wnętrza archiwum ZIP.

## Cel obecnego playtestu

W wersji **v0.1.0 Pre-Alpha** najważniejsze jest sprawdzenie, czy podstawowa pętla rozgrywki działa czytelnie i stabilnie: poruszanie się po świecie → interakcja z obiektami → podnoszenie i przenoszenie przedmiotów → korzystanie z ekwipunku i kontenerów → podstawowe systemy survivalowe.

Nie jest to jeszcze test finalnej grafiki, balansu ani ilości zawartości. Część assetów, interfejsu i elementów świata nadal będzie wymieniana lub rozwijana.

## Multiplayer — ważna informacja

System multiplayer oraz wymiana barterowa między graczami **działają już w wewnętrznych testach developerskich**, ale nie są jeszcze przygotowane do wygodnego użycia w obecnym publicznym buildzie.

Publiczny playtest v0.1.0 skupia się obecnie głównie na testach solo. Multiplayer, prosty sposób hostowania/dołączania do gry oraz barter dla testerów zostaną udostępnione w jednej z kolejnych wersji testowych.

## Co można obecnie testować

- poruszanie postacią i kamerą,
- interakcje kontekstowe ze świata gry,
- podnoszenie i odkładanie przedmiotów,
- ekwipunek uwzględniający masę, objętość i liczbę slotów,
- pojemniki, wóz oraz przenoszenie przedmiotów,
- podstawowe parametry przetrwania,
- testowe narzędzia, materiały i obiekty świata.

## Co zrobić jako tester

Jeśli chcesz pomóc, spróbuj przejść poniższe punkty i zapisz wszystko, co zachowuje się dziwnie lub nieczytelnie:

- [ ] Pobierz kilka różnych przedmiotów i sprawdź, czy poprawnie trafiają do ekwipunku.
- [ ] Odłóż przedmiot z powrotem do świata i sprawdź jego fizykę oraz możliwość ponownego podniesienia.
- [ ] Przenieś przedmioty pomiędzy ekwipunkiem a dostępnymi kontenerami.
- [ ] Sprawdź zachowanie ekwipunku przy większej liczbie przedmiotów oraz ograniczeniach masy/objętości.
- [ ] Użyj dostępnych obiektów interaktywnych i zwróć uwagę, czy komunikaty oraz klawisze są zrozumiałe.
- [ ] Pograj dłużej bez restartowania gry i zwróć uwagę na zacinanie interakcji, problemy z UI lub inne niestabilne zachowanie.
- [ ] Sprawdź, czy przedmioty nie wpadają pod mapę, nie zaczynają nadmiernie podskakiwać ani nie zachowują się niestabilnie.

Nie musisz zaliczać całej listy. Nawet jeden dobrze opisany problem jest pomocny.

## Jak zgłosić błąd

Przy zgłoszeniu podaj, jeśli możesz:

1. **Co robiłeś przed wystąpieniem problemu.**
2. **Co się stało.**
3. **Czego oczekiwałeś.**
4. Czy problem da się powtórzyć.
5. Screenshot lub krótki film, jeśli problem jest widoczny na ekranie.

Przykład:

```text
Problem: przedmiot zniknął po przeniesieniu do skrzyni.
Kroki: podniosłem Stone -> otworzyłem skrzynię -> przeniosłem Stone do kontenera.
Oczekiwane: Stone powinien pojawić się w skrzyni.
Wynik: zniknął z inventory, ale nie pojawił się w skrzyni.
Powtarzalność: 2/3 prób.
```

## Logi i crashe

Jeśli gra się zawiesi, zamknie albo wystąpi trudny do odtworzenia błąd, do zgłoszenia warto dołączyć najnowszy plik logu.

Typowa lokalizacja logów w Windows:

```text
%LOCALAPPDATA%\GearlSoul1\Saved\Logs
```

Raporty crashy, jeśli zostały utworzone:

```text
%LOCALAPPDATA%\GearlSoul1\Saved\Crashes
```

Najłatwiej wkleić powyższą ścieżkę bezpośrednio do paska adresu Eksploratora Windows.

## Status projektu

- **Wersja:** v0.1.0 Pre-Alpha Playtest
- **Platforma:** Windows 64-bit
- **Silnik:** Unreal Engine 5
- **Stan:** aktywny rozwój
- **Charakter buildu:** publiczny playtest — nie finalne wydanie
- **Multiplayer/barter:** działają wewnętrznie, publiczne testy zostaną udostępnione później

Pełna paczka jest publikowana w sekcji [Releases](https://github.com/Aniosek/GearSoul-Playtest/releases). To repozytorium służy do udostępniania publicznych wersji testowych; kod źródłowy gry nie jest tutaj publikowany.

## Integralność pobrania

SHA-256:

```text
CA8B8FCB76FCFAED9C35458ED94AD8C4B7C9D7FF74929AD2A87045B38A68DDB6
```

Plik z sumą kontrolną znajduje się również przy wydaniu.

## Informacja dla testerów

GearSoul znajduje się na wczesnym etapie produkcji. Grafika, interfejs, balans i zawartość mogą ulec zmianie. Najbardziej wartościowe są obecnie zgłoszenia dotyczące stabilności, interakcji, ekwipunku, fizyki przedmiotów oraz czytelności podstawowych systemów.

Dziękuję każdej osobie, która poświęci czas na sprawdzenie buildu i opisanie znalezionego problemu.

---

Copyright © 2026 Aniosek. Wszelkie prawa zastrzeżone. Publiczna paczka jest przeznaczona do testowania; nie udostępnia kodu źródłowego ani praw do zasobów projektu.
