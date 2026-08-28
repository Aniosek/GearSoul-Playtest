# GearSoul v0.2.3 — pełna checklista testera

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
- [ ] 41 pickupów można fizycznie zebrać.
- [ ] Masa, objętość i sloty są prawidłowo przeliczane.
- [ ] Plecak zwiększa pojemność dopiero po założeniu i nadal ma własną masę.
- [ ] Przedmioty leżą stabilnie i nie wystrzeliwują po zetknięciu z graczem.
- [ ] Kolejne wydobyte surowce zajmują osobne wolne miejsca zamiast tworzyć pionowy stos.

## Świat i produkcja

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

## Gracze i gospodarka

- [ ] Profesje rozwijają się dopiero przez wykonane czynności.
- [ ] Claim ogranicza budowę, rozbiórkę i infrastrukturę bez uprawnień.
- [ ] Barter wymaga dwóch prawdziwych graczy i akceptacji obu stron.
- [ ] Wóz ma fizyczny ładunek, części, masę i wpływ drogi.
- [ ] Karawana wymaga gracza, wozu i prawdziwego ładunku.
- [ ] Regiony różnią się dostępem do zasobów.

## Przetrwanie i medycyna

- [ ] Głód, pragnienie, energia i temperatura zmieniają się w czasie.
- [ ] Dzień/noc i kataklizmy są zgodne u hosta i klientów.
- [ ] Narzędzia zużywają się, a naprawa zużywa fizyczny materiał.
- [ ] Drugi gracz opatruje krwawienie LinenBandage.
- [ ] HerbalExtract leczy infekcję dopiero po opatrzeniu rany.
- [ ] Leczenie nie przywraca magicznie punktów HP.
- [ ] Śmierć kończy historię konkretnej postaci bez tworzenia NPC.

## Raport

Zapisz rolę (solo/host/klient), liczbę graczy, kroki, oczekiwany i faktyczny rezultat, powtarzalność oraz załącznik. Logi są zwykle w `%LOCALAPPDATA%\GearlSoul1\Saved\Logs`.
