# GearSoul v0.8.2 — kierunek i animowana lokomocja MetaHumana

Publiczna poprawka wersji pre-alpha do testów multiplayerowych Etapów 0–71.

## Najważniejsze zmiany

- MetaHuman jest teraz ustawiony przodem do rzeczywistego kierunku ruchu zamiast poruszać się bokiem,
- animowany Manny pozostaje niewidocznym sterownikiem ruchu, a zgodne kości jego pozy są kopiowane w czasie działania gry do szkieletu MetaHumana,
- miednica, nogi i obie stopy reagują na chód, bieg oraz skok hosta i klientów,
- walidacja runtime sprawdza rzeczywisty ruch stóp; jeśli animowana poza nie dotrze, gra pokazuje działającego Manny'ego zamiast nieruchomej postaci.

Poprawka nie zmienia autorytetu ruchu, kolizji, ekwipunku ani sieciowej tożsamości postaci. MetaHuman pozostaje warstwą wizualną istniejącej postaci multiplayerowej.

## Weryfikacja

- automatyzacja: 75/75 testów zakończonych sukcesem,
- trzy niezależne packaged smoke: w każdym uruchomiono serwer i dwóch klientów, czyli łącznie sześć instancji klientów,
- dodatkowy smoke test z czystej paczki publikacyjnej: sukces,
- host i klienci potwierdzili właściwy kierunek postaci oraz animowany ruch miednicy i obu stóp,
- końcowa paczka jest sprawdzana pod kątem braku PDB, kodu źródłowego, zapisów gry i edytowalnych źródeł MetaHuman.
- archiwum zostało próbnie rozpakowane mechanizmem Windows; potwierdzono 53 pliki, obecność EXE i pełne 1 826 740 192 bajty zawartości.

## Zawartość publiczna

Publiczne repozytorium zawiera dokumentację, a paczka wydania wyłącznie skompilowane pliki wykonywalne oraz ugotowane, zaszyfrowane kontenery Unreal Pak/IoStore. Kod źródłowy C++, pliki PDB, edytowalne źródła assetów i źródłowa zawartość MetaHuman nie są publikowane.

## Instalacja

1. Pobierz ZIP i rozpakuj go w całości.
2. W rozpakowanym folderze uruchom `START_GearSoul_Solo.bat`, `START_GearSoul_Host.bat` albo `START_GearSoul_Join.bat`.
3. Nie uruchamiaj EXE bezpośrednio z wnętrza archiwum.

Suma SHA-256 jest publikowana w `SHA256SUMS.txt` oraz jako osobny plik przy wydaniu GitHub Release.
