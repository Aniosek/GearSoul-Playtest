# GearSoul — publiczna roadmapa

## Aktualny status — 0.9.20, 19.09.2026

**Pre-alpha. Etap 100 jest NIEUKOŃCZONY. Beta jeszcze się nie rozpoczęła.** Numery dawnych etapów i wersji nie są procentem ukończenia gry. Beta nastąpi po domknięciu animacji, pozostałych mechanik i sprawdzeniu grywalności; bez obiecywania daty.

Obecna wersja ma trzy mapy, wycinany las i górskie kopalnie, fizyczną budowę, barter, transport, produkcję, survival, głos przestrzenny, profil oraz odrębne pule 50 Wiedzy / 40 Rozwoju. Najnowsze przyrosty to budowana kuźnia, dymarka i skrzynia, wiadro, posłanie, siedzący odpoczynek oraz przesuwanie mebli. Zakres i ograniczenia: [instrukcja 0.9.20](README_PL.md).

### Kolejność dalszych prac

1. Pełne animacje snu, podejścia, niesienia i pracy; integracja z wnętrzami i sterowaniem.
2. Pozostałe osobno budowane wyposażenie magazynu żywności i produkcji, pełne łańcuchy wytwarzania.
3. Domknięcie gildii i rozwoju osad; doprecyzowanie zasad racji żywnościowych.
4. Uzgodniona ochrona i zagrożenia postaci pozostawionej offline, bez karania za wyłączony serwer.
5. Transakcyjny transfer gracza, wozu i towarów między niezależnymi serwerami. Trzy mapy nie są jeszcze takim transferem.
6. Dalszy szlif terenu, modeli, UI i balansu; profilowanie większych grup i długich zapisów świata.
7. Hosting, rozmowa na fizycznych komputerach i sesje z testerami; dopiero po spełnieniu kryteriów grywalności wejście w beta testy.

Roadmapa opisuje kierunek, a nie gwarantowane daty. Kolejność może zmienić się po testach. Poniżej zachowano **historyczną numerację z v0.8.2**, która nie opisuje aktualnego stanu ukończenia.

## Etapy 1–71 — COMPLETED

Fundament C++ i multiplayer, fizyczne przedmioty, przetrwanie, dzień/noc, zbieranie zasobów, budowanie i rozbiórka, claimy, barter, wozy, drogi, kopalnie, metalurgia, rolnictwo, regiony, karawany, trwały świat, reputacja, medycyna, kataklizmy, narzędzia, kooperacyjna budowa, woda, zwierzęta transportowe, osady, mosty, odnawianie lasu, naprawialne wyposażenie, regionalne magazynowanie żywności, Punkty Wiedzy, działki osad, budynki graczy, informacja o XP, fizyczne zlecenia między graczami, prawdziwe członkostwo i role osady, gospoda, uprawy, gotowanie, konserwacja żywności, właściwy ładunek wozu, ręczne ciągnięcie, wpływ nawierzchni na transport, ceny wynikające z prawdziwych transakcji, fizyczne kontrakty przewozowe między regionami oraz trzy warstwy odzieży z moknięciem, suszeniem i ochroną przed pogodą.

Wydanie v0.8.2 jest poprawką jakościową istniejącego zakresu Etapów 1–71, a nie nowym etapem: porządkuje kierunek postaci i przekazuje animowaną lokomocję do MetaHumana z bezpiecznym fallbackiem, potwierdzonym testami multiplayer gotowej paczki.

## Etapy 72–75 — IN DEVELOPMENT

- Etap 72: schronienie i wpływ rodzaju budynku na ochronę przed pogodą.
- Etap 73: choroby, infekcje oraz leczenie zależne od stanu postaci i realnych środków.
- Etap 74: ciężkie urazy i konsekwencje wymagające pomocy innych graczy.
- Etap 75: rozszerzona pogoda i pory roku spięte z temperaturą, uprawami, podróżą i pracą.

## Etapy 76–82 — PLANNED

- Przestrzenny voice chat i narzędzia bezpieczeństwa społeczności.
- Bard, występy oraz dobrowolne wsparcie gracza przez innych graczy.
- Role tłumaczy, organizacja karawan i komunikacja między społecznościami.

## Etapy 83–88 — PLANNED

- Oddzielne mapy/regiony działające w lokalnej symulacji.
- Transakcyjny transfer postaci, karawany, pojazdu i ładunku między serwerami.
- Ochrona przed utratą i duplikacją przedmiotów podczas timeoutu lub rozłączenia.

## Etapy 89–100 — PLANNED

- Domknięcie permanent death z ochroną przed śmiercią techniczną.
- Stabilność, bezpieczeństwo gospodarki oraz testy obciążenia.
- Playtest 10–30 prawdziwych graczy i poprawki wynikające z ich zachowań.
- Kryteria ukończenia 100/100 systemów core gameplay bez udawania finalnej oprawy.
