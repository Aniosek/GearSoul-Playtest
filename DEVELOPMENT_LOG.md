# GearSoul — publiczny dziennik rozwoju

## 2026-08-30

- Opublikowano v0.4.0 z mapą naturalną, responsywnym ekwipunkiem i screenami.
- Oficjalne buildy UE 5.8 zakończyły się powodzeniem; automatyzacja uzyskała 63/63.
- Zapakowany serwer oraz dwóch klientów przeszły smoke test.
- Po zgłoszeniu testera rozpoczęto poprawę kolizji wzgórz i osadzenia drzew.
- Dodano generator paczki diagnostycznej, szablon zgłoszenia oraz publiczny opis wizji projektu.

Ten plik opisuje rezultaty i decyzje, nie publikuje kodu źródłowego ani prywatnych danych projektu.

## 2026-09-01

- Ukończono etapy 60–62: pierwszą działającą osadę, przygotowanie gleby oraz uprawy zależne od warunków.
- Poprawiono gwałtowne obracanie zwierząt i potwierdzono płynny, ograniczony skręt.
- Dodano prawdziwych członków i role osady, warunek pięciu graczy oraz kooperacyjną gospodę.
- Pola wymagają fizycznej pracy, wody, ziaren i opcjonalnego kompostu; pogoda, chwasty i choroby wpływają na plon.
- Build, 70/70 testów oraz test finalnej paczki z hostem i dwoma klientami zakończyły się sukcesem.

## 2026-09-06

- Ukończono Etapy 69–70: rynek regionalny oparty na transakcjach graczy i fizyczne kontrakty transportowe.
- Zintegrowano zoptymalizowaną postać Epic MetaHuman jako warstwę wizualną bez przenoszenia autorytetu ruchu i ekwipunku poza istniejącą postać sieciową.
- Dodano autorskie modele etapów wykonania kamiennych narzędzi oraz wyposażenie warsztatu: kuźnię, miechy i skrzynię.
- Poprawiono kolejność ładowania modułu MetaHuman, a końcowe gotowanie przeszło bez ostrzeżenia o brakującej klasie komponentu.
- Build, 73/73 testy automatyczne i smoke test czystej paczki Windows zakończyły się sukcesem.

## 2026-09-07 — v0.8.1

- Ukończono Etap 71: trzy fizyczne warstwy odzieży, moknięcie, suszenie i ochrona przed pogodą.
- Każde ubranie zachowuje własną wilgotność, trwałość, jakość i tożsamość; mokra odzież izoluje słabiej, ale żadna kombinacja nie daje pełnej odporności na środowisko.
- Burza moczy warstwy od zewnątrz, pogoda bez opadów je osusza, a rozpalone ognisko przyspiesza proces do sześciu razy bez nowego ciągłego przeliczania każdej klatki.
- Poprawiono rozdzielenie plecaka od ubrań oraz ustabilizowano pozycję startową drugiego gracza w teście karawany.
- Build, 75/75 testów, regresja hosta i dwóch klientów, restart zapisu, gotowanie oraz smoke test finalnego EXE zakończyły się sukcesem.

## 2026-09-08 — v0.8.2

- Audyt lokomocji rozdzielił dwie przyczyny ślizgania: nieprawidłowy kierunek warstwy wizualnej oraz brak skutecznego przekazania animowanej pozy do szkieletu MetaHumana.
- MetaHuman otrzymał właściwy kierunek względem ruchu, a animowany Manny pozostał sterownikiem, z którego zgodne kości są kopiowane w czasie działania gry.
- Walidacja runtime sprawdza ruch miednicy i obu stóp; jeśli poza nie dociera, gracz zobaczy działającego Manny'ego zamiast nieruchomej postaci.
- Automatyzacja zaliczyła 75/75 testów. Trzy niezależne packaged smoke objęły po jednym serwerze i dwóch klientów, czyli łącznie sześć instancji klientów; dodatkowy smoke przeszedł z czystej paczki publikacyjnej.
- Publiczne wydanie zawiera tylko skompilowane pliki wykonywalne i ugotowane, zaszyfrowane kontenery Unreal Pak/IoStore. Kod C++, PDB, edytowalne źródła assetów i źródłowa zawartość MetaHuman pozostają prywatne.
