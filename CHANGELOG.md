# GearSoul — changelog

## v0.9.10 — 2026-09-13

- Kudłate zwierzęta z animowanymi łapami i sierścią, po trzy w każdym regionie.
- Wędka z długą linką, łowiska, przynęta, surowy i pieczony pstrąg, receptury i XP łowienia.
- Pochodnia z paliwem, płomieniem i światłem z cieniami; księżyc i nocne oświetlenie istniejących domów.
- Obraz Leszka w domu w Alderen.
- Poprawki sztywnych łap, wiązania sierści, podwójnego spławika, orientacji płomienia i zdjęcia oraz obsługi anulowania/pełnego plecaka przy łowieniu.
- 127/127 testów projektu; pełny zakres kontroli paczki i ograniczenia: [opis 0.9.10](RELEASE_v0.9.10.md). To nadal pre-alpha.

## v0.9.9 — 2026-09-13

- Trzy regiony: Alderen, Sairen, Norvak; Alderen jako mapa domyślna, osobny launcher wyboru regionu i trybu gry.
- F10: wybór mikrofonu i wyjścia, lokalny odsłuch do 15 s, miernik, głośność głosu i dźwięk w tle dla dwóch okien. Brak automatycznego nagrywania lub nadawania.
- Fizyczne dostawy na budowę, noszenie ciężkich materiałów, profil i osobne pule wiedzy/rozwoju.
- Prototypowe drążenie zamkniętej skały z podporami budowanymi z przynoszonych kłód. Bez ukończonej podpory nie ma dalszego postępu.
- 126/126 testów projektu; trzy regiony i głos sprawdzone również w wykonywalnej paczce. Szczegóły i jawne ograniczenia w [opisie 0.9.9](RELEASE_v0.9.9.md). To nie gotowe 1.0.0.

## v0.9.5 — 2026-09-11

- Aktualny przyrost projektu do lokalnego etapu 95, nie 95% ukończenia całej gry.
- Poprawiona animacja ścinania oburącz: IK, kierunek barków, praca bioder/kolan, kontakt ostrza z pniem i krótkie wyhamowanie. Zachowana autoryzacja trafienia przez serwer i anulowanie pracy.
- Aktualne narzędzia kamienne, miedziane, żelazne i stalowe, osobne części, montaż i trwałość; nowe przedmioty użytkowe i wyposażenie osady.
- Księga testowa, fizyczny wóz i zaprzęg, schronienie we wnętrzach oraz kolejne poprawki odtwarzania stanu świata. Launchery wydania nadal domyślnie wyłączają trwały zapis.
- 112/112 testów automatycznych projektu. Szczegółowe wyniki kontroli paczki oraz instrukcja: [opis v0.9.5](RELEASE_v0.9.5.md).

## v0.8.3 — 2026-09-10

- Etap 72 i nowy dom średniowieczny: dwie izby, sześć widocznych warstw modelu, trzy poziomy LOD i uproszczone kolizje.
- Osiem etapów dostaw i pracy, ciosanie złączy przed kołkowaniem, gwoździe dopiero na późniejszych etapach; 54 cykle pracy i normalna pojemność plecaka.
- Fizyczna partia 120 gwoździ z łupki żelaznej, paliwa i czterech cykli młotka po rozgrzaniu.
- Proceduralny ruch prawej ręki podczas pracy i test przejść przez rzeczywisty model domu.
- 80/80 testów automatycznych oraz pełna budowa w gotowym EXE. ZIP rozpakowany i zweryfikowany: 57 zgodnych plików.
- Meble i drzwi są jeszcze statyczne; odtworzenie zbudowanych domów po restarcie świata pozostaje do domknięcia.

## v0.8.2 — 2026-09-08

- poprawiono kierunek warstwy wizualnej MetaHumana, aby postać była ustawiona przodem do rzeczywistego ruchu,
- animowana poza Manny'ego jest kopiowana w czasie działania gry do zgodnych kości MetaHumana, dzięki czemu miednica, nogi i stopy reagują na chód, bieg oraz skok,
- walidacja runtime wykrywa brak rzeczywistego ruchu stóp i bezpiecznie odsłania animowanego Manny'ego zamiast pozostawiać nieruchomą postać,
- 75/75 testów automatycznych, trzy packaged smoke z łącznie sześcioma klientami oraz dodatkowy smoke z czystej paczki zakończyły się powodzeniem,
- paczka publiczna zawiera wyłącznie skompilowane pliki i ugotowane, zaszyfrowane dane Unreal Pak/IoStore — bez kodu źródłowego, PDB i edytowalnych źródeł assetów lub MetaHuman.
- archiwum przepakowano ze ścieżkami zgodnymi z Eksploratorem Windows; po próbnym rozpakowaniu potwierdzono komplet 53 plików.

## v0.8.1 — 2026-09-07

- Etap 71: trzy fizyczne warstwy odzieży — bazowa, ocieplająca i zewnętrzna,
- indywidualna wilgotność ubrań, moknięcie od warstwy zewnętrznej podczas burzy i osłabienie izolacji po przemoczeniu,
- naturalne suszenie oraz suszenie do 6× szybsze przy rozpalonym ognisku,
- bezpieczna zamiana ubrania w tej samej warstwie, niezależne wyposażenie plecaka i walidacja całego zestawu,
- migracja trwałego zapisu do schematu 3 z zachowaniem zgodności starszych suchych przedmiotów,
- 75/75 testów automatycznych, udany `BuildCookRun`, regresja multiplayer i smoke test finalnego EXE.

## v0.8.0 — 2026-09-06

- Etapy 69–70: regionalne ceny oparte na rzeczywistych transakcjach graczy oraz fizyczne kontrakty transportowe z escrow,
- zoptymalizowany MetaHuman Medium/JointsOnly jako nowa warstwa wizualna postaci,
- autorskie, modułowe kamienne narzędzia i etapy ich wykonania,
- autorska kuźnia, miechy i skrzynia warsztatowa z trzema poziomami LOD,
- poprawiona kolejność ładowania MetaHumanSDKRuntime bez ostrzeżenia podczas gotowania,
- 73/73 testy automatyczne, udany `BuildCookRun` oraz smoke test czystego EXE z kodem 0.

## v0.7.1 — 2026-09-02

- dodano fizyczne zbiory, spichlerz, gotowanie oraz suszenie, solenie, wędzenie i fermentację,
- wóz otrzymał fizyczną linę mocującą, przeciążenie i uszkodzenia osi oraz obu kół,
- dodano ręczne ciągnięcie lekkiego wozu do 200 kg z realnym kosztem energii,
- wysiłek człowieka i zwierzęcia, prędkość oraz zużycie pojazdu zależą od nawierzchni,
- mapa zawiera cztery podpisane rodzaje drogi i komplet stanowisk Etapów 0–68,
- oficjalny build, 71/71 testów, spakowany serwer z dwoma klientami, restart zapisu i obciążenie 2/5/10/15 klientów zakończyły się powodzeniem.

## v0.7.0 — 2026-09-01

- poprawiono gwałtowne obracanie zwierząt dzięki zachowaniu kierunku i limitowi prędkości skrętu,
- dodano rzeczywistych członków oraz role osady bez generowania zastępczych NPC,
- działająca osada wymaga pięciu graczy, magazynu, domu, warsztatu i gospody,
- dodano fizyczną, kooperacyjną budowę gospody,
- rozbudowano przygotowanie gleby, podlewanie i nawożenie skończonym kompostem,
- wzrost i plon reagują na pogodę, porę roku, wilgotność, żyzność, chwasty i choroby,
- oficjalny build UE 5.8, 70/70 testów automatycznych i smoke test spakowanej wersji z hostem oraz dwoma klientami zakończyły się powodzeniem.

## v0.6.0 — 2026-08-31

- fizyczna Tablica Zleceń Graczy z blokadą prawdziwej nagrody w escrow,
- przyjmowanie pracy, częściowe dostawy ciężkich materiałów, atomowa wypłata i magazyn odbioru,
- trwały zapis zlecenia i obu magazynów potwierdzony testem restartu,
- polska informacja o XP za zweryfikowaną pracę,
- stabilne prowadzenie zaprzęgniętego wołu oraz płynniejszy ruch stad,
- 66/66 testów automatycznych, test dwóch klientów oraz test finalnej spakowanej wersji.

## v0.5.0 — 2026-08-31

- Punkty Wiedzy z ograniczonym budżetem specjalizacji,
- fizyczny obszar działki osady i uprawnienia budowlane,
- kooperacyjna budowa domu i kuźni z rzeczywistych materiałów i pracy młotkiem.

## v0.4.1 — 2026-08-31

- usunięcie przenikalnego pierścienia wzgórz, zmniejszenie mapy testowej i dodanie twardej granicy,
- poprawa osadzenia drzew przy gruncie,
- generator paczki diagnostycznej dla testerów,
- formularz błędu GitHub i publiczna dokumentacja wizji.

## v0.4.0

- naturalny teren, rzeka, las i lekkie stylizowane drzewa,
- responsywny polski ekwipunek,
- odnawianie lasu i skutki wycinki,
- fizyczna budowa mostu,
- zaawansowane żelazne narzędzia i naprawy,
- regionalne magazynowanie oraz psucie żywności,
- 63/63 automatycznych testów oraz multiplayerowy smoke test zapakowanej wersji.

## v0.3.0

- jakość i oczyszczanie wody,
- zwierzęta transportowe oraz stado,
- osady i usługi zależne od infrastruktury graczy.

Starsze publiczne wydania i ich opisy pozostają dostępne w sekcji Releases.
