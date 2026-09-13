# GearSoul v0.9.10 Pre-Alpha — zwierzęta, łowienie i nocne światło

To wersja testowa, nie gotowe 1.0. Numer wydania nie oznacza procentu ukończenia gry.

## Dodane

- Nowy kudłaty zwierzak z psim pyskiem i wydłużonym ciałem, poruszającymi się łapami oraz sierścią związaną z animowaną skórą. Po trzy w Alderen, Sairen i Norvak.
- Wędka bez współczesnego kołowrotka, z długą linką do spławika na wodzie. Po jednym łowisku z paleniskiem w każdym regionie.
- Łowienie na przynętę, surowy i pieczony pstrąg, zużywanie wędki, XP łowienia oraz receptury składników i narzędzi.
- Pochodnia: zapalanie, paliwo do 600 sekund, animowany płomień, ciepłe światło i cienie w otoczeniu.
- Księżyc i światło nocne. Światła w 20 istniejących domach każdego regionu, związane z konkretnymi budynkami.
- Oprawione zdjęcie Leszka w jednym domu w Alderen.

## Poprawione

- Zwierzęta zapisane na mapie odtwarzają poprawnie pozę szkieletu; łapy nie pozostają sztywne podczas przemieszczania.
- Sierść deformuje się razem z animowaną skórą, zamiast pozostawać w nieruchomej pozie.
- Naprawiono inicjalizację materiału sierści przy pierwszym wyświetleniu w gotowym EXE (przygotowanie PSO przed rejestracją komponentu).
- Do paczki dołączono brakującą zależność systemu włosów, aby silnik nie próbował szukać jej poza spakowaną grą.
- Wędka podczas zarzucenia nie pokazuje dodatkowego, schowanego spławika. Po anulowaniu przywraca model złożony.
- Łowienie kontroluje serwer. Wczesne anulowanie, odejście, schowanie wędki i rozłączenie zwalniają stanowisko; nie blokują ruchu.
- Pełny plecak odmawia rozpoczęcia łowienia przed zabraniem przynęty. Udany połów dodaje jedną rybę i zużywa jeden punkt trwałości wędki.
- Poprawione kierunek płomienia, ustawienie obrazu w domu oraz powiązanie świateł z rozbiórką budynku.
- Palenisko ryb ma kamienny model zamiast szarej bryły.

## Co testować

1. Wędka w dłoni + ciasto w plecaku → E przy łowisku → branie po 5–11 sekundach → E w ciągu 6 sekund. Sprawdź też anulowanie, odejście i pełny plecak.
2. Surowy pstrąg + paliwo + sprawny świder ogniowy → pieczenie przy palenisku przez 25 sekund. Surowa ryba nie jest bezpośrednio jadalna.
3. Pochodnia w dłoni + sprawny świder ogniowy → L. Sprawdź światło na ścianie, gaszenie po schowaniu i spójny widok drugiego gracza.
4. Noc w każdym regionie, wejścia do domów, światło i cienie. Porównaj chód nowych zwierząt z bliska i z daleka.
5. Host i klient muszą używać 0.9.10. Stare zapisy zachowaj, ale test uruchom z dołączonych launcherów bez trwałego zapisu.

## Weryfikacja

Projekt: kompilacja Succeeded, regresja **127/127**, 0 błędów i 0 pominiętych. Testy działania nowych interakcji zaliczone na trzech regionach; Alderen dodatkowo oceniony w renderowanej grze. Osobny serwer i klient zaliczyły zapalenie/replikację pochodni oraz połów ze zgodnym stanem przedmiotów po obu stronach.

Końcowy build Windows: **Succeeded**. Kontrola trzech regionów wykonywalnej gry zakończyła się wynikiem 0 niepowodzeń w każdym regionie (Alderen z renderowaniem; Sairen i Norvak bez renderowania). Nie wystąpiły wcześniejszy błąd PSO sierści ani brakująca zależność HairStrands.

Gotowy **host listen-server + osobny klient** zaliczyły zapalenie pochodni, replikację i połów przez zwykłe interakcje klienta. Po obu stronach: jedna ryba, dwie pozostałe przynęty i trwałość wędki 79. Klient został uruchomiony głównym EXE z kontrolnie rozpakowanego ZIP-a. Test wykonano lokalnie, nie przez Internet.

Archiwum ma **1 833 198 947 bajtów (1,83 GB)** i **50 plików**. Zostało rozpakowane do nowego folderu; każdy plik porównano z buildem przy użyciu SHA-256. Nazwy wpisów ZIP używają separatora `/`, poprawnego dla Eksploratora Windows. Brak nowych screenów, źródeł projektu, osobnych plików zdjęcia, modeli Blender i prywatnych zapisów.

SHA-256 ZIP: `8c9c3bfd78d240fc3a1ce770214e80f70f78d67a0a4681c488458a2af8ad1721`.

## Ograniczenia

- Brak nowej pełnej animacji rzutu wędką, dźwięków pochodni oraz obrażeń od ognia. Płomień jest animowanym materiałem, nie symulacją wolumetryczną.
- Księżyc to prosty dysk atmosferyczny bez tekstury kraterów.
- Światła rozmieszczono w istniejących domach map; nie są automatycznie dodawane do każdego przyszłego domu gracza.
- Sierść ma LOD i wyłączoną symulację fizyczną, ale nadal wymaga profilowania GPU. Nie potwierdzono płynności 15 renderujących klientów ani połączeń WAN tej wersji.
- Regiony pozostają oddzielnymi mapami, nie gotowym transferem między niezależnymi serwerami. Pozostałe ograniczenia pre-alpha nadal obowiązują.

## Pobieranie i zgłoszenia

Pobierz `GearSoul_v0.9.10_PreAlpha_Multiplayer_Windows.zip` z załączników wydania i rozpakuj cały ZIP do nowego folderu. Nie pobieraj automatycznego „Source code” jako gry. Start: `GearlSoul1.exe` (Alderen) lub `START_GearSoul_Regiony.bat` (wybór regionu/hosta).

Błędy: **gearsoul00@gmail.com** lub [GitHub Issues](https://github.com/Aniosek/GearSoul-Playtest/issues). Podaj wersję, region, host/klient i kroki odtworzenia. `CREATE_BUG_REPORT_PACKAGE.bat` przygotuje pliki diagnostyczne; przejrzyj ZIP przed wysłaniem, bo logi mogą zawierać adresy IP i nazwy katalogów. Ta aktualizacja nie zawiera nowych screenów.
