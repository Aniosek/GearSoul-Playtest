# GearSoul v0.7.0 — pełna checklista testera

## Start i multiplayer

- [ ] Solo uruchamia właściwą mapę.
- [ ] Host może chodzić i grać, a nie tylko uruchamiać serwer.
- [ ] Klient w LAN dołącza po IPv4 hosta.
- [ ] Co najmniej dwóch klientów widzi ruch, interakcje i zmiany świata.
- [ ] Zamknięcie jednego klienta nie blokuje pozostałych.

## Sterowanie i interakcja

- [ ] WASD, kamera, skok, kucanie, sprint i zoom działają.
- [ ] Mysz w górę kieruje kamerę w górę; oś pozioma pozostaje normalna.
- [ ] Celowany obiekt ma czytelny komunikat interakcji.
- [ ] `E` otwiera właściwy panel i nie blokuje postaci po jego zamknięciu.

## Inventory i materia

- [ ] Start zawiera tylko FireDrill, StonePickaxe i MasonryHammer.
- [ ] 48 przedmiotów z galerii można fizycznie zebrać.
- [ ] Masa, objętość i sloty są prawidłowo przeliczane.
- [ ] Plecak zwiększa pojemność dopiero po założeniu i nadal ma własną masę.
- [ ] Przedmioty leżą stabilnie i nie wystrzeliwują po zetknięciu z graczem.
- [ ] Kolejne wydobyte surowce zajmują osobne wolne miejsca zamiast tworzyć pionowy stos.

## Świat i produkcja

- [ ] Naturalny teren, drzewa, rzeka i droga wczytują się poprawnie bez szarej pustej planszy.
- [ ] Ekwipunek mieści się na ekranie 1600×900, tekst się nie nakłada, a przyciski pozostają dostępne.
- [ ] Drzewa, kłody, opał i ognisko tworzą pełny fizyczny ciąg.
- [ ] Glina przechodzi przez mokrą, suszoną i wypaloną cegłę.
- [ ] Fundament, zaprawa, mur, palisada i rozbiórka działają.
- [ ] Żelazo przechodzi przez rudę, przygotowanie, bloomery i kowalstwo.
- [ ] Pszenica przechodzi przez suszenie, młyn, ciasto i chleb.
- [ ] Kamień, żelazo i węgiel można wydobywać bez zablokowania postaci.
- [ ] Ścinanie, kopanie i wydobycie zużywają energię oraz durability i nie przyjmują spamu szybszego niż cooldown.
- [ ] Drugi gracz widzi wyposażone narzędzie oraz jego ruch podczas pracy.
- [ ] Plac palisady wymaga dokładnie 5 kłód i 5 cykli młotka.
- [ ] Plac fundamentu wymaga dokładnie 4 kamieni i 6 cykli młotka.
- [ ] Materiały można donosić na plac pojedynczo, a wcześniejsze dostawy nie znikają po odejściu gracza.
- [ ] Dwóch uprawnionych graczy może wspólnie dostarczać materiały i pracę przy jednym placu.
- [ ] Naprawa uszkodzonej konstrukcji zużywa pasujący materiał, energię i durability młotka.
- [ ] Alchemia tworzy fizyczny eliksir maskujący, a efekt jest czasowy.
- [ ] Surowa woda ma jakość, oczyszczanie zużywa opał, a beczka zachowuje fizyczne porcje.
- [ ] Trzy jelenie poruszają się jako stado bez humanoidalnych NPC.
- [ ] Jelenie i wół skręcają płynnie, nie wirują ani nie zmieniają gwałtownie kierunku co kilka klatek.
- [ ] Karmienie i pojenie zwierzęcia zużywa dokładnie jedną realną porcję.
- [ ] Wół daje się przypiąć do wozu i ciągnie go wyłącznie podczas prowadzenia przez gracza.
- [ ] Ścięty las można odnowić fizyczną sadzonką, a skutki dla gleby pozostają zapisane.
- [ ] Most przyjmuje osiem osobnych kłód, wymaga młotka i blokuje przeciążony wóz.
- [ ] Żelazne narzędzia można złożyć i naprawić z właściwej głowicy oraz trzonka.
- [ ] Suche magazyny i chłodne piwnice inaczej wpływają na świeżość żywności.

## Gracze i gospodarka

- [ ] Profesje rozwijają się dopiero przez wykonane czynności.
- [ ] Komunikat XP pojawia się krótko nad postacią, która naprawdę wykonała pracę, i ma polską nazwę zawodu.
- [ ] Punkty Wiedzy mają ograniczony budżet i nie pozwalają jednej postaci odblokować wszystkich specjalizacji.
- [ ] Claim ogranicza budowę, rozbiórkę i infrastrukturę bez uprawnień.
- [ ] Barter wymaga dwóch prawdziwych graczy i akceptacji obu stron.
- [ ] Wóz ma fizyczny ładunek, części, masę i wpływ drogi.
- [ ] Karawana wymaga gracza, wozu i prawdziwego ładunku.
- [ ] Regiony różnią się dostępem do zasobów.
- [ ] Plac osady przyjmuje osobno 1 zestaw sztandaru, 4 kłody i 4 kamienie.
- [ ] Prawdziwy gracz może dołączyć do osady i otrzymuje zapisaną rolę; system nie tworzy mieszkańców NPC.
- [ ] Osada staje się działająca dopiero przy pięciu członkach oraz po rejestracji magazynu, domu, warsztatu i gospody.
- [ ] Plac gospody przyjmuje 10 osobnych kłód i 12 poprawnych cykli młotkiem wykonywanych wspólnie przez graczy.
- [ ] Woda, magazyn, barter i naprawy stają się usługą osady dopiero po rejestracji istniejącej infrastruktury.
- [ ] Autor zlecenia wpłaca trzy prawdziwe srebrne monety do Tablicy Zleceń.
- [ ] Inny gracz przyjmuje zlecenie i dostarcza dwie kłody pojedynczo.
- [ ] Ostatnia dostawa wypłaca dokładnie trzy monety wykonawcy, a kłody czekają na autora.
- [ ] Anulowanie nieprzyjętego zlecenia zwraca nagrodę, ale nie tworzy kopii przedmiotów.
- [ ] Restart świata zachowuje otwarte zlecenie, postęp dostaw i zawartość escrow.

## Gleba i uprawy

- [ ] Pole przyjmuje trzy pełne cykle pracy łopatą przed siewem.
- [ ] Suche pole wymaga fizycznej porcji wody, a wysiew zużywa dokładnie cztery ziarna.
- [ ] Zepsute jedzenie użyte jako kompost znika z ekwipunku i zwiększa żyzność zamiast tworzyć darmowy nawóz.
- [ ] Susza i upał obniżają wilgotność, burza ją zwiększa, a ochłodzenie wywołuje stres pogodowy.
- [ ] Zaniedbane pole zbiera chwasty lub chorobę; pielęgnacja zużywa pracę i poprawia stan pola.
- [ ] Jakość oraz wielkość zbioru zależą od wilgotności, żyzności, pory roku, pogody, chwastów i chorób.

## Przetrwanie i medycyna

- [ ] Głód, pragnienie, energia i temperatura zmieniają się w czasie.
- [ ] Dzień/noc i kataklizmy są zgodne u hosta i klientów.
- [ ] Narzędzia zużywają się, a naprawa zużywa fizyczny materiał.
- [ ] Drugi gracz opatruje krwawienie LinenBandage.
- [ ] HerbalExtract leczy infekcję dopiero po opatrzeniu rany.
- [ ] Leczenie nie przywraca magicznie punktów HP.
- [ ] Śmierć kończy historię konkretnej postaci bez tworzenia NPC.

## Żywność, wóz i drogi — v0.7.1

- [ ] Zebrane ziarno można wysuszyć, zapakować do worka i umieścić w spichlerzu bez tworzenia darmowych porcji.
- [ ] Gotowanie gulaszu zużywa mięso, wodę, paliwo i sprawny zapłon, a po ukończeniu zwraca ten sam garnek.
- [ ] Suszenie, solenie, wędzenie i fermentacja mają różne fizyczne składniki, czasy oraz produkty.
- [ ] Załadowany wóz nie rusza bez fizycznej liny, a zdjęcie liny zwraca ten sam stos.
- [ ] Człowiek może chwycić dyszel tylko przy zabezpieczonym ładunku do 200 kg i traci energię podczas ciągnięcia.
- [ ] Cięższy wóz wymaga wołu; ręczny ciągnący i zwierzę nie napędzają go równocześnie.
- [ ] Ścieżka, droga ziemna, utwardzona i kamienna dają zauważalnie różny wysiłek, prędkość i zużycie kół.
- [ ] Puszczenie dyszla, oddalenie, utrata energii lub uszkodzenie wozu nie blokują ruchu postaci.

## Raport

Zapisz rolę (solo/host/klient), liczbę graczy, kroki, oczekiwany i faktyczny rezultat, powtarzalność oraz załącznik. Logi są zwykle w `%LOCALAPPDATA%\GearlSoul1\Saved\Logs`.

Raport wyślij na **[gearsoul00@gmail.com](mailto:gearsoul00@gmail.com)**. Nie dołączaj publicznego adresu IP ani danych konta.
