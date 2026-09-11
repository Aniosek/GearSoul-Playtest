# GearSoul v0.9.5 — ścinanie oburącz, narzędzia i osada

Nowa paczka Windows z aktualnym stanem lokalnych etapów do 95. Numer wersji nie oznacza 95% ukończenia gry.

## Najważniejsze zmiany

- Poprawiona istniejąca animacja ścinania: dwie dłonie prowadzone przez IK, właściwy skręt barków i bioder, ugięcie kolan, odsunięcie głowicy od głowy oraz krótki stop po kontakcie ostrza z pniem.
- Energia, zużycie i obrażenia pozostają autoryzowane przez serwer. Szybkie powtarzanie interakcji nie tworzy dodatkowych trafień; odejście lub schowanie siekiery przerywa pracę.
- Aktualny zestaw narzędzi z kamienia, miedzi, żelaza i stali, ich części i montaż, warsztat oraz modele przedmiotów użytkowych.
- Aktualna mapa: budynki osady i ich schronienie, księga przywoływania próbek, wóz z częściami i zwierzęta pociągowe, nowe wyposażenie i kolejne poprawki mechanik.

## Pobranie i test

Pobierz **GearSoul_v0.9.5_PreAlpha_Multiplayer_Windows.zip** z załączników wydania i rozpakuj całość. Automatyczny „Source code” nie zawiera gry.

Uruchom `START_GearSoul_Solo.bat`, `START_GearSoul_Host.bat` lub `START_GearSoul_Join.bat`. Host i wszyscy klienci muszą używać tej samej wersji. Launchery włączają świeży scenariusz bez trwałego zapisu.

Najpierw sprawdź ścinanie E przy pniu, chwyt z kilku stron, anulowanie zamachu, zużycie siekiery i obserwację drugiego gracza. Następnie warsztat/montaż, barter, zaprzęg, schronienie i księgę testową. Szczegóły: [instrukcja testera](https://github.com/Aniosek/GearSoul-Playtest/blob/main/README_PL.md).

## Weryfikacja projektu

- 112/112 testów automatycznych.
- Dwie próby rzeczywistej animacji: odległość 115 i 135 cm od środka drzewa, trzy kamery, razem 150 pomiarów chwytu. Brak wykrytego odstępu punktów riggu od trzonka w badanej fazie zamachu, kontaktu i wycofania. Pomiary punktów nie zastępują oceny całej powierzchni skóry.
- Serwer z dwoma klientami przy 100 ms opóźnienia i 3% utraty pakietów: interakcja klienta, replikacja fazy, jedno trafienie; również księga, warsztat i transport.

## Weryfikacja gotowej paczki Windows

- Kompilacja, przygotowanie zasobów i pakowanie: **BUILD SUCCESSFUL**.
- Animacja uruchomiona w gotowym EXE: trzy kąty kamery, 75 pomiarów riggu, 25 zaliczonych kontroli i brak zgłoszonego błędu próby ścinania.
- ZIP: **50 plików**, **1 612 846 629 bajtów**. Po kontrolnym rozpakowaniu porównano sumy SHA-256 wszystkich plików.
- Z rozpakowanego EXE uruchomiono hosta i zdalnego klienta lokalnego przy symulacji 100 ms opóźnienia i 3% utraty pakietów. Zaliczone: księga, warsztat, replikacja produktu i fazy ścinania, pojedyncze trafienie oraz cykle prowadzenia zaprzęgu.
- Dodatkowo host z dwoma klientami z rozpakowanej paczki: ruch MetaHumanów i replikacja kuźni/warsztatu/spichlerza oraz naprawy, prowadzenie zaprzęgu, informacja o doświadczeniu, zlecenia, zabezpieczona pożyczka, odzież i schronienie. Próby ruchu i mechanik wykonano w osobnych uruchomieniach, ponieważ scenariusz zleceń teleportuje uczestników. Obie fazy zakończyły się powodzeniem.
- SHA-256 ZIP-a: `21502cea4b844d74a0bf6fc7bc74f3e910b5f7bfcce6dbd0e619c67fb66b9890`.

## Ograniczenia wydania

To pre-alpha. Pozostałe pełne animacje pracy i część wyposażenia nadal wymagają rozwoju. Nie potwierdzono nowego profilu GPU dla 15 graczy ani testu WAN. To nie jest trwały serwer produkcyjny. Nie usuwaj swoich starszych zapisów.

Zgłoszenia: **gearsoul00@gmail.com** lub [Issues](https://github.com/Aniosek/GearSoul-Playtest/issues). Podaj wersję 0.9.5, rolę host/klient, kroki i screenshot. Paczkę diagnostyczną przejrzyj przed wysłaniem: logi mogą zawierać adresy IP i nazwy lokalnych katalogów.

Wydanie zawiera skompilowaną grę i ugotowane zasoby, bez źródłowych modeli MetaHuman, plików PDB i prywatnych kluczy.
