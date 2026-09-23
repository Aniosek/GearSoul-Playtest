# GearSoul v0.9.21 — księga podróżnika

Publiczny **Pre-Alpha Multiplayer Playtest** dla Windows. To nie beta ani ukończone 1.0.0.

## Co zmieniono

- Ekwipunek, profil postaci, rozwój i dźwięk otrzymały wspólny wygląd otwartej średniowiecznej księgi.
- Lewa strona ekwipunku zawiera masę, objętość, miejsca i sloty. Prawa strona zawiera nazwę, ikonę, stan, parametry oraz działania wybranego przedmiotu.
- Prawa karta ekwipunku została odsunięta od grzbietu.
- Siatka profesji kończy się przed grzbietem; Ciesielstwo i Rolnictwo nie nachodzą już na prawą stronę.
- „Rozwój · cechy” oraz wszystkie cztery cechy mieszczą się na lewej stronie, a prawa służy szczegółom wyboru.
- Dołączono krój Cormorant Garamond i pełny tekst licencji SIL OFL 1.1.

## Kontrola wydania

- kompilacja Editor Win64 Development: zaliczona;
- kompilacja Game Win64 Development: zaliczona;
- gotowanie czterech map: zaliczone, 0 błędów;
- 148/148 testów `GearlSoul`: zaliczone, 0 błędów, 0 ostrzeżeń testów;
- ZIP rozpakowany i porównany plik po pliku: 59/59 zgodnych;
- test księgi w rozpakowanym EXE: profil, rozwój, ekwipunek i odzyskanie sterowania — zaliczone.

## Paczka

- plik: `GearSoul_v0.9.21_PreAlpha_Playtest_Windows.zip`;
- rozmiar: 1 851 607 026 bajtów;
- SHA-256: `de933c37b71ecf7fb248e6c0910e7607dc2afd0512e4ca0709ab5b74845e369f`.

Rozpakuj ZIP do nowego folderu. Host i klienci muszą używać tej samej wersji. Kod źródłowy i edytowalne źródła assetów nie są częścią paczki.

## Co szczególnie sprawdzić

1. Otwórz ekwipunek i wybieraj przedmioty o długich nazwach oraz opisach. Tekst prawej karty nie powinien wchodzić w grzbiet.
2. Otwórz profil (`P`) i przewiń listę zawodów. Ciesielstwo, Rolnictwo i kolejne karty powinny pozostać po lewej stronie.
3. Przełącz „Rozwój · cechy”. Cztery cechy powinny mieścić się na lewej stronie, a opis na prawej.
4. Sprawdź rozdzielczość 1920×1080 oraz mniejsze okno. Księga powinna skalować się bez obcinania.
5. Zamknij panel przez `Esc`, `P`, `I` i `X`; ruch i kamera muszą zostać odzyskane.

Pozostałe mechaniki i jawne ograniczenia są opisane w [README_PL.md](README_PL.md). Błędy zgłaszaj w GitHub Issues lub na **gearsoul00@gmail.com**.
