# GearSoul v0.9.10 — Pre-Alpha Multiplayer Playtest

To wydanie testowe, **nie gotowa gra 1.0.0**. Numer nie oznacza procentu ukończenia. Poniżej są instrukcje bieżącej paczki; dalsza historia opisuje starsze wydania.

## Uruchomienie 0.9.10

Pobierz archiwum Windows z [wydania 0.9.10](https://github.com/Aniosek/GearSoul-Playtest/releases/tag/v0.9.10) i rozpakuj je w całości do nowego folderu. Nie uruchamiaj EXE wewnątrz ZIP. Unreal Editor nie jest potrzebny. Host i klienci muszą używać tej samej wersji; nie mieszaj plików 0.9.9 i 0.9.10.

- `GearlSoul1.exe` lub `START_GearSoul_Solo.bat` — region **Alderen**.
- `START_GearSoul_Regiony.bat` — Alderen, Sairen albo Norvak; wybierz solo lub hosta.
- `START_GearSoul_Host.bat` — host Alderen; `START_GearSoul_Join.bat` — adres IP hosta, niezależnie od wybranego regionu.
- `TEST_Mechanik_Stara_Plansza.bat` — dodatkowa, stara plansza kontrolna; nie jest regionem ani domyślną mapą.
- Dla Internetu nadal potrzebne jest połączenie z hostem na UDP 7777; automatyczne zaproszenia/NAT traversal nie są gotowe.

Launchery uruchamiają test **bez trwałego zapisu**. Nie kasuj starszych zapisów. Regiony to oddzielne mapy, nie działający transfer pomiędzy niezależnymi serwerami.

## Nowości 0.9.10 — zwierzęta, łowienie i światło

- Po trzy nowe kudłate zwierzęta i jednym łowisku z paleniskiem w każdym regionie. To fikcyjne zwierzę z psim pyskiem i wydłużonym ciałem, nie pies o imieniu „Kuna”.
- Wędka ma dłuższą linkę prowadzącą od końca kija do spławika na wodzie. Przy łowisku weź wędkę do dłoni, miej ciasto jako przynętę i naciśnij **E**. Po komunikacie o braniu naciśnij **E** ponownie. Wczesne E anuluje, tak samo odejście lub schowanie wędki.
- Branie następuje po 5–11 sekundach; okno wyciągnięcia trwa 6 sekund. Połów daje jednego pstrąga, 10 XP łowienia i zużywa 1 punkt trwałości wędki. Pełny plecak powinien odmówić rozpoczęcia bez zabrania przynęty.
- Surowy pstrąg nie jest bezpośrednio jadalny. Przy palenisku przygotuj surową rybę, paliwo i sprawny świder ogniowy; pieczenie trwa 25 sekund.
- **L** zapala lub gasi pochodnię trzymaną w dłoni. Do zapalenia potrzebny jest sprawny świder ogniowy. Pełna pochodnia wystarcza na 600 sekund; schowanie, pływanie lub śmierć ją gaszą.
- Pochodnia oświetla postać i otoczenie, z cieniami. Księżyc daje światło nocne. Istniejące domy na mapach mają ciepłe światła; w jednym domu w Alderen jest obraz Leszka.
- Przedmioty i składniki znajdziesz w księdze testowej; dodano również receptury wędki i pochodni. Udźwig nadal obowiązuje.

**Co poprawiono:** ruch łap zwierząt zapisanych na mapie, dopasowanie sierści do animowanej skóry, podwójny spławik podczas łowienia, orientację płomienia i zdjęcia w domu. Światła domowe są powiązane z rozbiórką domu. Łowienie jest kontrolowane przez serwer i nie blokuje ruchu przy anulowaniu.

**Granice tej wersji:** nie ma nowej pełnej animacji rzutu wędką, dźwięków pochodni ani obrażeń od ognia. Księżyc jest prostym dyskiem bez tekstury kraterów. Światła rozmieszczono w istniejących domach mapy — nie są jeszcze automatycznym wyposażeniem każdego nowego domu gracza. Sierść wymaga dalszego profilowania GPU; nie potwierdzono płynności 15 renderujących klientów. Testuj najpierw na dwóch komputerach.

## Mikrofon, słuchawki i dwa okna na jednym komputerze

**F10** otwiera ustawienia dźwięku; przycisk jest też w plecaku. Wybierz mikrofon i wyjście słuchawkowe. „Test słuchawek” odtwarza krótki ton. „Test mikrofonu — 15 s” pokazuje poziom sygnału i daje lokalny odsłuch. Używaj słuchawek, żeby uniknąć sprzężenia. Test nie zapisuje nagrania i nie wysyła go innym; kończy się po 15 sekundach, zamknięciu panelu lub utracie aktywności okna.

Do rozmowy obaj gracze muszą włączyć głos, zamknąć menu i zbliżyć postacie na mniej niż 25 m. Mówiący przytrzymuje **V**. W drugim oknie włącz „Dźwięk także w nieaktywnym oknie” (domyślnie włączone). Nie przełączaj aktywnego okna podczas nadawania: przechwytywanie zatrzymuje się dla prywatności. Zwykła rozmowa nie odtwarza własnego głosu. Włączenie czatu jest świadomą decyzją w każdej sesji; sam wybór urządzenia nie uruchamia mikrofonu.

## Co sprawdzić w tej wersji

1. Głos host ↔ klient, poprawne urządzenia, wyciszenie gracza, zasięg, odsłuch lokalny i dźwięk w tle.
2. Trzy regiony: grunt, wejścia i schronienie w budynkach, ruch zwierząt, interaktywne zasoby przy osadzie. Dalszy las jest w dużej części dekoracyjny.
3. Kopalnia zaczyna się od zamkniętej skały. Po wykuciu odcinka dostarcz pojedynczo 3 kłody, obrób połączenia siekierą i zamocuj młotkiem. Dopiero ukończona podpora otwiera dalsze drążenie. Prototyp ma 6 odcinków / 12 m; brak swobodnych rozgałęzień, prawdziwych zawałów i docelowego oświetlenia pod ziemią.
4. Budowanie od podstaw: dostawy pojedynczych materiałów, noszenie ciężkich kłód, kolejne etapy pracy, meble oraz studnia. Nie ma automatycznej skrzyni dostaw. Nie wszystkie meble mają jeszcze dodatkowe funkcje użytkowe.
5. Profil **P**: osobne profesje i praktyka, pula do 50 Punktów Wiedzy i osobno do 40 Punktów Rozwoju. Limity nie oznaczają przyznania pełnej puli na starcie.
6. Barter, budowa i wydobycie we dwójkę: brak powielania surowców, spójny stan i odzyskanie sterowania po zamknięciu interakcji.

Nie potwierdzamy wydajności 15 renderujących klientów ani odsłuchu mowy na każdej konfiguracji sprzętu. Zacznij od dwóch komputerów. Szczegółowe wyniki gotowej paczki są w opisie wydania.

**Błędy:** `CREATE_BUG_REPORT_PACKAGE.bat`, potem przejrzyj ZIP przed wysłaniem (logi mogą zawierać IP, nazwy katalogów i zapis świata). Wyślij na **gearsoul00@gmail.com** albo do GitHub Issues. Podaj 0.9.10, mapę, host/klient, urządzenia audio i kroki odtworzenia.

---

## Archiwum: v0.9.5 — Pre-Alpha Multiplayer Playtest

To jest wczesna, techniczna wersja testowa GearSoul. Nie jest jeszcze reprezentacją końcowej grafiki, balansu ani zawartości. Celem wydania jest sprawdzenie fizycznego świata, interakcji między prawdziwymi graczami i stabilności multiplayera.

## Pobranie i uruchomienie

1. Pobierz `GearSoul_v0.9.5_PreAlpha_Multiplayer_Windows.zip` z sekcji **Releases**.
2. Rozpakuj całe archiwum. Nie uruchamiaj gry wewnątrz pliku ZIP.
3. Windows może pokazać ostrzeżenie dla niepodpisanej wersji pre-alpha. Paczka nie ma instalatora i nie zmienia systemu.
4. Uruchom jeden z plików:
   - `START_GearSoul_Solo.bat` — test solo,
   - `START_GearSoul_Host.bat` — host rozgrywki,
   - `START_GearSoul_Join.bat` — dołączenie do hosta.

W sieci lokalnej wpisz adres IPv4 komputera hosta. Przy teście przez Internet host musi dopuścić grę w Zaporze Windows i przekierować **UDP 7777** na swoim routerze. GearSoul używa na razie listen-servera — komputer hosta jest również jednym z graczy.

## Aktualne wydanie v0.9.5 — co testować

1. **Ścinanie:** weź sprawną siekierę, podejdź blisko pnia (do 1,35 m od jego środka), stań przodem i użyj interakcji E. Obie dłonie powinny trzymać trzonek; ostrze trafia w pień, krótko wyhamowuje i wraca. Obrażenia są naliczane przy trafieniu, nie przy rozpoczęciu zamachu. Sprawdź odejście, schowanie narzędzia i szybkie powtarzanie E — nie powinno być dodatkowego trafienia ani blokady ruchu.
2. **Narzędzia i warsztat:** porównaj kamienne, miedziane, żelazne i stalowe siekiery, kilofy oraz młotki. Sprawdź odrębne głowice, trzonki, wiązania/kliny, etap montażu, zużycie składników i trwałość. Większa trwałość materiału nie oznacza braku zużycia.
3. **Księga testowa:** przywołuj potrzebne rzeczy na oznaczonym polu zamiast szukać wszystkich próbek porozrzucanych po mapie. Udźwig i objętość nadal obowiązują. To pomoc testowa, nie docelowa gospodarka gry.
4. **Osada:** sprawdź wnętrza i schronienie w domu, kuźni, warsztacie, spichlerzu i gospodzie. Budowa wymaga wskazanych materiałów, kwalifikacji i narzędzia. Komunikat rozbiórki nie powinien zastępować zwykłego opisu, gdy nie trzymasz młotka.
5. **Transport i multiplayer:** zaprzęgnij własne zwierzę do wozu, rozpocznij/zatrzymaj prowadzenie kilka razy, przełóż ładunek. Drugi tester powinien widzieć ten sam stan. Sprawdź barter, warsztat i ścinanie jednocześnie z drugą osobą; szukaj utraty lub powielania przedmiotów.

Przed publikacją projektu: 112/112 testów automatycznych, kontrola chwytu w grze z trzech kamer przy dwóch dystansach oraz serwer z dwoma klientami przy 100 ms opóźnienia i 3% straty pakietów. Wyniki testów gotowej paczki podajemy osobno w opisie wydania GitHub.

### Ograniczenia i bezpieczeństwo testów

- To nadal pre-alpha, a numer 0.9.5 nie oznacza 95% ukończenia całej gry.
- Pełna choreografia jest poprawiana stopniowo; animacja ścinania nie oznacza gotowych pełnych animacji kopania, kucia i podnoszenia. Część wyposażenia ma nadal funkcję dekoracyjną.
- Dostarczone launchery uruchamiają świeży scenariusz **bez trwałego zapisu**. Nie kasuj swoich starszych zapisów. W projekcie rozwijane są osobne mechanizmy odtwarzania świata, ale ta paczka nie jest trwałym serwerem produkcyjnym.
- Nie potwierdzono profilu wydajności 15 renderujących graczy ani testu połączeń przez Internet dla tego wydania. Zacznij od dwóch komputerów i małej grupy.
- Błędy wysyłaj na **gearsoul00@gmail.com** lub GitHub Issues. Podaj wersję 0.9.5, czy byłeś hostem/klientem, kroki odtworzenia i screenshot. `CREATE_BUG_REPORT_PACKAGE.bat` zbiera diagnostykę; przejrzyj archiwum przed wysłaniem — logi mogą zawierać adresy IP i nazwy lokalnych katalogów.

## Historia wydań (poniższe opisy dotyczą wskazanych starszych wersji)

### v0.8.3: dom budowany etapami

- Dom z kamiennym fundamentem, drewnianym szkieletem, glinianymi ścianami i dachem krytym gontem. W środku izba ze stołem i ławami oraz komora z łóżkiem i skrzynią.
- Osiem etapów: fundament → ciosanie złączy → szkielet i kołkowanie → ściany → łupanie gontów → mocowanie dachu → stolarka → wyposażenie.
- Łącznie: 6 kamieni, 14 kłód, 8 porcji gliny, 18 kutych gwoździ i 54 cykle pracy. Materiały dostarcza się po jednej sztuce; nie trzeba nosić całego domu w plecaku.
- Potrzebne są kwalifikacje ciesielskie (poziom 1 i jeden przydzielony punkt wiedzy), sprawny młotek oraz narzędzie wskazane przy danym etapie: siekiera lub łopata.
- Przy placu budowy stoi wspólna skrzynia z ograniczonym zapasem testowym. Odkładaj zbędne narzędzia, żeby zmieścić pełnowymiarową kłodę. Pojemność plecaka nie została zwiększona.
- Kuźnia obok przyjmuje łupkę żelazną i paliwo. Po rozgrzaniu i czterech cyklach młotka można odebrać 120 gwoździ. To fizyczna partia, nie nieskończone źródło.
- Schronienie chroni przed deszczem i temperaturą; zniszczony budynek chroni słabiej.

### Co sprawdzić

1. Wejdź do gotowego domu, obejdź stół, przejdź do drugiej izby i wróć na zewnątrz.
2. Buduj drugi dom z innym testerem. Oboje powinni widzieć ten sam etap; niewłaściwe materiały i narzędzia nie mogą zastępować wymaganych.
3. Sprawdź, czy dostawy znikają tylko z plecaka dostawcy i trafiają do wspólnego postępu budowy.
4. Obserwuj pracę ręki, zużycie narzędzia i energii. Nie powinno być blokady sterowania po pracy.
5. Wykuj gwoździe i użyj ich na dachu. Sprawdź odbiór, masę oraz przenoszenie do skrzyni.

Drzwi i okiennice są obecnie stałymi elementami ustawionymi w pozycji otwartej. Meble są oprawą, bez spania i osobnego otwierania skrzyni we wnętrzu. Odtworzenie zbudowanych domów po pełnym restarcie świata nadal wymaga osobnego domknięcia systemu zapisu — nie traktuj tej paczki jako trwałego serwera produkcyjnego.

## Poprawka v0.8.2

- MetaHuman jest ustawiony przodem do rzeczywistego kierunku ruchu i nie jedzie już bokiem,
- animowany Manny pozostaje niewidocznym sterownikiem ruchu, a zgodne kości jego pozy są kopiowane w czasie działania gry do szkieletu MetaHumana,
- nogi, miednica oraz pozostałe wspólne kości reagują na chód, bieg, skok i ruch innych graczy także w multiplayerze,
- gra sprawdza po uruchomieniu, czy poza samym przypięciem animacji poza faktycznie dotarła do obu stóp; w razie awarii automatycznie pokazuje działającego Manny'ego zamiast nieruchomej postaci,
- trzy powtórzenia testu końcowej paczki z serwerem i dwoma klientami potwierdziły właściwy kierunek `-90°`, realne przyspieszenie, ruch dokładnie do przodu oraz pracę stóp w kolejnych klatkach na obu klientach; nie wystąpił fallback ani błąd krytyczny, a pełna automatyka zaliczyła 75/75 testów.

## Co zmieniło się w v0.8.1

- ukończono Etap 71: trzy niezależne warstwy odzieży — bazową, ocieplającą i zewnętrzną,
- dodano lnianą koszulę spodnią, wełnianą tunikę i skórzany płaszcz jako fizyczne przedmioty o własnej masie, objętości, jakości, trwałości, GUID-zie i wilgotności,
- burza moczy odzież od warstwy zewnętrznej do wewnętrznej, a odporność na wodę ogranicza tempo nasiąkania bez zapewniania pełnej odporności,
- mokra odzież traci część izolacji; sucha odzież spowalnia wpływ zimna i gorąca na ciało, ale nigdy nie daje całkowitej niewrażliwości,
- ubrania schną podczas pogody bez opadów i znacznie szybciej przy rozpalonym ognisku,
- założenie drugiego ubrania tej samej warstwy atomowo zastępuje poprzednie, a plecak pozostaje niezależnym wyposażeniem,
- wilgotność i stan założenia są replikowane oraz zapisują się razem z dokładnym fizycznym stosem; zapis ze starszej wersji jest migrowany jako suchy,
- mapa zawiera po dwa egzemplarze każdego ubrania przy ognisku oraz polską instrukcję testu,
- pełna regresja zaliczyła 75/75 testów, test mapy z serwerem i dwoma klientami, pełną regresję multiplayer oraz restart trwałego zapisu.

Warstwy są obecnie czytelnie pokazane w interfejsie i działają mechanicznie. Zmiana widocznego stroju MetaHumana będzie osobnym etapem oprawy; ten build nie udaje, że prototypowy przedmiot leżący na ziemi jest końcowym modelem ubrania.

## Co zmieniło się w v0.8.0

- ukończono Etapy 69–70: ceny między osadami wynikające z ofert prawdziwych graczy oraz fizyczne kontrakty transportowe powiązane z karawaną,
- manekin testowy został zastąpiony w grze zoptymalizowanym MetaHumanem klasy Medium; dotychczasowy szkielet nadal bezpiecznie steruje ruchem i socketami narzędzi,
- dodano autorskie, modułowe modele kamiennych narzędzi i etapów ich wykonania: osobny kamień, trzonek, wiązanie oraz ukończone warianty,
- dodano autorskie stanowiska warsztatowe: kuźnię, miechy kowalskie i skrzynię warsztatową, każde z trzema poziomami LOD,
- narzędzia w ręku, obiekty świata, kuźnia, barter i magazyny korzystają z nowych modeli bez przenoszenia ciężkiej geometrii do fizyki serwera,
- pełna regresja po zmianie postaci i oprawy zaliczyła 73/73 testy automatyczne.

## Co zmieniło się w v0.7.1

- ukończono Etapy 63–68: zbiory i spichlerz, gotowanie, cztery metody konserwacji żywności, właściwy wóz, ręczne ciągnięcie i drogi,
- wóz przechowuje fizyczny ładunek, linę mocującą oraz stan osi i obu kół; przeciążenie realnie wpływa na ruch i zużycie,
- lekki, zabezpieczony wóz do 200 kg może ciągnąć człowiek, zużywając własną energię; cięższy wymaga zwierzęcia pociągowego,
- błoto, teren leśny, góry i śnieg kosztują więcej wysiłku i szybciej zużywają pojazd niż droga ziemna, utwardzona lub kamienna,
- mapa pokazuje cztery podpisane odcinki nawierzchni, pełny łańcuch zbiorów, gotowania i konserwacji oraz wszystkie stanowiska Etapów 0–68,
- ponowny audyt zaliczył 71/71 testów, serwer z dwoma klientami, restart zapisu i obciążenie 2/5/10/15 klientów.

## Co zmieniło się w v0.6.0

- nad postacią pojawia się krótka, polska informacja o XP zdobytym za prawdziwie wykonaną pracę,
- prowadzenie zaprzęgniętego wołu jest stabilnym trybem: ponowne użycie kończy prowadzenie, ale nie rozprzęga wozu,
- ruch stad został wygładzony częstszymi, mniejszymi krokami bez zwiększania ich prędkości,
- na mapie stoi fizyczna **Tablica Zleceń Graczy**; nie tworzy zadań ani pieniędzy przez NPC,
- autor blokuje w tablicy trzy prawdziwe srebrne monety i zleca dostarczenie dwóch kłód,
- drugi gracz przyjmuje pracę i wnosi ciężkie kłody pojedynczo, więc nie musi mieścić obu naraz w ekwipunku,
- ostatnia dostawa atomowo wypłaca nagrodę, a kłody czekają na autora w fizycznym magazynie tablicy,
- zlecenie, dostawy i escrow są zapisywane razem ze światem; test restartu potwierdził odtworzenie bez utraty lub duplikacji monet.

## Co zmieniło się w v0.5.0

- dodano trwały budżet Punktów Wiedzy: dwa punkty startowe, maksymalnie 50 na postać i pięć w jednej profesji,
- ukończony sztandar pokazuje nieblokujący pierścień rzeczywistej działki osady,
- gracze z prawem `Build` mogą stawiać wewnątrz działki fizyczne place domu i kuźni,
- dom wymaga specjalizacji ciesielskiej, ośmiu osobnych kłód oraz dziesięciu cykli pracy młotkiem,
- kuźnia łączy specjalizacje murarską i kowalską, dziesięć kamieni oraz dwanaście cykli pracy młotkiem,
- gotowe konstrukcje nie tworzą darmowych zapasów, NPC ani automatycznej produkcji,
- mapa zawiera gotowy dom, kuźnię i osobne place obu budynków do szybkiego testu.

## Poprawki zachowane z v0.4.1

- usunięto zawieszony pierścień wzgórz, zmniejszono mapę testową i dodano twardą granicę obszaru,
- drzewa dekoracyjne i ścinane są osadzane podstawą przy gruncie,
- niedostępna interakcja z drzewem pokazuje konkretny powód zamiast ogólnego komunikatu,
- dołączono generator paczki diagnostycznej z logami, raportami awarii i zapisem gry.

- mapa testowa ma naturalny teren, rzekę, las i lekkie, stylizowane drzewa zamiast samej szarej planszy,
- interfejs ekwipunku został przebudowany i poprawnie skaluje się między innymi w rozdzielczości 1600×900,
- las pamięta wycinkę, stan gleby, erozję i sadzonki; nie odradza drzew za darmo,
- most wymaga ośmiu fizycznych kłód i pracy młotkiem, a przeciążony wóz nie może po nim bezpiecznie jechać,
- kuźnia wytwarza i naprawia żelazny kilof, siekierę oraz młotek z fizycznych głowic i trzonków,
- trzy regiony mają fizyczne magazyny żywności, różne warunki składowania i prawdziwe psucie partii,
- chleb, mięso, zepsute jedzenie, mąka i ciasto otrzymały czytelne, lekkie wizualizacje w surowym stylu,
- nowe modele jedzenia mieszczą się w małym budżecie renderingu i nie uczestniczą w fizyce serwera swoją siatką.

## Najważniejsze rzeczy do sprawdzenia

- Czy host i pozostali gracze widzą swoje ruchy, interakcje i zmiany świata.
- Czy MetaHuman obu graczy stoi na ziemi, płynnie chodzi, obraca się bez skręcania kończyn i prawidłowo trzyma narzędzia w prawej dłoni.
- Czy kamienna siekiera, kilof, łopata i młotek pokazują kolejne fizyczne części wykonania oraz pasują skalą do dłoni i świata.
- Czy kuźnia, miechy i skrzynia warsztatowa zachowują czytelny surowy styl oraz nie powodują zauważalnych przycięć.
- Czy lnianą koszulę spodnią, wełnianą tunikę i skórzany płaszcz można podnieść przy ognisku oraz założyć z ekwipunku.
- Czy interfejs pokazuje dokładnie trzy różne warstwy, wilgotność każdego ubrania, łączną izolację i ochronę przed deszczem.
- Czy ponowne użycie założonego ubrania je zdejmuje, a ubranie tej samej warstwy zastępuje poprzednie bez utraty przedmiotu.
- Czy `GSTestCataclysm Storm 30 1` stopniowo moczy ubrania, mokra wełna daje mniej izolacji, a `GSTestCataclysm Clear` rozpoczyna suszenie.
- Czy przy rozpalonym ognisku ubrania schną szybciej i ich wilgotność nie spada poniżej 0% ani nie rośnie powyżej 100%.
- Czy drugi klient widzi zmiany stanu wyposażenia, a po restarcie zapisu zachowane są założone warstwy oraz ich wilgotność.
- Czy każdy nowy gracz zaczyna tylko z `FireDrill`, `StonePickaxe` i `MasonryHammer`.
- Czy 48 przedmiotów w galerii można podnosić i czy masa, objętość oraz sloty zmieniają się poprawnie.
- Czy wodę da się oczyścić i przełożyć do beczki bez utraty jakości i pochodzenia.
- Czy jelenie trzymają się stada, a karmienie i pojenie zużywa dokładnie jedną fizyczną porcję.
- Czy wół daje się przypiąć do wozu i nie wykonuje transportu bez prowadzącego gracza.
- Czy po zabezpieczeniu ładunku liną lekki wóz daje się chwycić za dyszel, podąża fizycznie za graczem i nie blokuje postaci po puszczeniu.
- Czy wóz z ładunkiem przekraczającym 200 kg odmawia ręcznego ciągnięcia i wymaga wołu.
- Czy te same odległości na ścieżce, drodze ziemnej, utwardzonej i kamiennej różnią się prędkością, kosztem energii i zużyciem kół.
- Czy plac osady przyjmuje 1 sztandar, 4 kłody i 4 kamienie pojedynczo oraz rejestruje tylko istniejącą infrastrukturę.
- Czy ukończony sztandar pokazuje nieblokujący pierścień działki, a dom i kuźnię można postawić wyłącznie wewnątrz niego z prawem `Build`.
- Czy `H` tworzy plac domu/kuźni, `Y` zmienia wybór, a materiały i pracę można dostarczać etapami przez kilku graczy.
- Czy ciężkie rzeczy leżą stabilnie, nie obracają się nienaturalnie i nie wystrzeliwują po dotknięciu postacią.
- Czy plecak zwiększa pojemność dopiero po fizycznym założeniu.
- Czy drzewa dają kłody, kłody można przerabiać na opał, a ognisko zużywa fizyczne paliwo.
- Czy glina przechodzi przez formowanie, suszenie i wypalanie cegły.
- Czy działa wydobycie kamienia, żelaza i węgla oraz czy po wyczerpaniu złoża postać nie zostaje zablokowana.
- Czy budowanie, rozbiórka i naprawa wymagają właściwych materiałów, narzędzi, profesji i uprawnień claimu.
- Czy skrzynia, barter, wóz, części wozu, drogi, magazyn węgla i karawany działają między graczami.
- Czy rolnictwo, suszenie ziarna, młyn, ciasto i piec chlebowy dają fizyczne produkty.
- Czy bochenek, surowe mięso, zepsute jedzenie, mąka i ciasto są rozpoznawalne, mają rozsądną skalę i nie wpadają w postać.
- Czy suchy magazyn i chłodna piwnica inaczej wydłużają świeżość właściwych partii, a zepsute jedzenie nie znika.
- Czy ścięty las można odnowić fizyczną sadzonką i czy skutki dla gleby pozostają zapisane.
- Czy most przyjmuje osiem osobnych kłód, wymaga młotka oraz blokuje przeciążony wóz.
- Czy żelazne narzędzia zużywają durability, dają się naprawić właściwą głowicą i zachowują swój identyfikator.
- Czy drugi gracz może opatrzyć krwawienie bandażem i dalej leczyć infekcję ekstraktem; leczenie nie może magicznie przywracać HP.
- Czy komunikat XP pojawia się tylko nad postacią, która wykonała zweryfikowaną pracę, i używa polskiej nazwy zawodu.
- Czy wół po rozpoczęciu i zakończeniu prowadzenia nadal pozostaje przypięty do tego samego wozu.
- Czy autor z trzema srebrnymi monetami może wystawić na tablicy zlecenie na dwie kłody, a drugi gracz przyjąć je i dostarczyć kłody po jednej sztuce.
- Czy nagroda jest wypłacana dopiero po drugiej kłodzie, a autor może odbierać ciężką dostawę pojedynczo.
- Czy dzień/noc, głód, pragnienie, energia, temperatura i zdarzenia środowiskowe są synchronizowane.
- Czy po śmierci jednej postaci drugi gracz nadal działa, a zakończona historia postaci nie odradza się bez ograniczeń.

## Test zdarzeń i komendy pomocnicze

Na mapie testowej otwórz konsolę klawiszem `~`, wpisz `GSTestHelp` i naciśnij Enter. Najważniejsze przykłady:

```text
GSTestStatus
GSTestInventory
GSTestGo Resources
GSTestGo Trade
GSTestCataclysm Heatwave 10 0.75
GSTestCataclysm Storm 10 0.75
GSTestCataclysm Clear
GSTestProfessions
GSTestProfessionXP Woodworking 100
GSTestKnowledge
GSTestSpendKnowledge Woodworking
```

Komendy `GSTest*` są wyłącznie narzędziem tej wersji testowej. Zapis świata jest domyślnie wyłączony w launcherach multiplayer, aby każdy test zaczynał się w porównywalnym stanie.

## Profesje i most

Praktyczna praca już rozwija osobne profesje. Ścięcie jednego drzewa wymaga czterech poprawnych uderzeń i daje łącznie 20 XP leśnictwa. Poziom 1 wymaga 100 XP, czyli około pięciu drzew. Obrabianie kłód rozwija osobno ciesielstwo (`Woodworking`); most wymaga ciesielstwa na poziomie 1.

Podczas szybkiego testu mapy można wpisać `GSTestProfessionXP Woodworking 100`, aby odblokować pracę przy moście albo domu bez powtarzania całej pętli produkcyjnej. Punkty Wiedzy są już osobnym, trwałym budżetem specjalizacji: postać zaczyna z dwoma, zdobywa kolejne przez zweryfikowane poziomy zawodów, może wydać maksymalnie pięć w jednej profesji i 50 w całym życiu. `GSTestKnowledge` pokazuje stan, a `GSTestSpendKnowledge Woodworking` przydziela punkt. Punkty nie zastępują XP ani rzeczywistej praktyki.

## Jak zgłosić błąd

Najłatwiej uruchomić `CREATE_BUG_REPORT_PACKAGE.bat`. Skrypt tworzy w folderze `BugReports` archiwum ZIP zawierające dostępne logi, raporty awarii i zapis gry. Nie zmienia ani nie usuwa oryginalnych danych.

Przed wysłaniem przejrzyj ZIP — log sieciowy może zawierać lokalny adres IP lub nazwę użytkownika w ścieżce. Gotowy raport możesz:

- dodać do [formularza błędu GearSoul na GitHubie](https://github.com/Aniosek/GearSoul-Playtest/issues/new?template=bug_report.yml), przeciągając ZIP do pola załączników,
- wysłać na **gearsoul00@gmail.com**.

W zgłoszeniu podaj:

- solo, host czy klient,
- ilu graczy było połączonych,
- co zrobiłeś krok po kroku,
- co miało się wydarzyć, a co wydarzyło się naprawdę,
- zrzut ekranu lub krótki film,
- log z `GearlSoul1\Saved\Logs`, jeśli powstał.

Nie przesyłaj publicznie adresu IP, danych konta ani innych prywatnych informacji.

## Stan i prawa

- Wersja: **v0.8.2 Pre-Alpha Multiplayer Playtest (Etapy 0–71 + poprawka animacji postaci)**
- Platforma: Windows 64-bit
- Silnik: Unreal Engine 5.8
- Kod źródłowy nie jest częścią paczki testowej.
- Zawartość gry jest spakowana przez Unreal Pak/IoStore. Jak w każdej aplikacji uruchamianej na komputerze użytkownika nie da się zagwarantować absolutnej niemożliwości analizy plików.
- Informacje o wykorzystanych zasobach CC0 i licencjonowanej zawartości Epic znajdują się w `THIRD_PARTY_NOTICES.txt`.

Copyright © 2026 Aniosek — kod i autorska zawartość GearSoul. Paczka służy do testowania i nie udziela praw do kodu ani autorskich zasobów projektu. Wskazane zasoby zewnętrzne zachowują własny status CC0.

Oprogramowanie, Unreal Engine i licencjonowana zawartość są udostępniane w tej wersji testowej „tak jak są”, bez dodatkowych zapewnień ani gwarancji. W maksymalnym zakresie dozwolonym przez prawo autor projektu wyłącza odpowiedzialność dotyczącą licencjonowanej technologii i zawartości podmiotów trzecich.
