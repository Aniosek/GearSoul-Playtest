# GearSoul v0.9.10-nightfix — jaśniejsza noc

Poprawka do 0.9.10 Pre-Alpha. To pełna paczka Windows, nie nakładka i nie gotowe 1.0.
Zawiera dotychczasowe trzy regiony, zwierzęta, łowienie, pochodnie i pozostałe systemy.

## Co poprawiono

- Nocą łatwiej zobaczyć drogę, teren i zarysy drzew oraz budynków.
- Rozjaśnione światło księżyca i otoczenia, łagodniejsza adaptacja do ciemności.
- Noc nadal jest ciemna, pochodnia pomaga, a oświetlone wnętrza zachowują ciepłe światło i cienie.
- Jasność dnia, zegar regionalny, zużycie pochodni i mechaniki rozgrywki pozostają bez zmian.

## Co przetestować

1. W każdym regionie przejdź nocą po drodze bez pochodni, następnie z zapaloną pochodnią.
2. Wejdź do oświetlonego domu i wyjdź z niego; zwróć uwagę na widoczność i adaptację jasności.
3. Sprawdź teren pod drzewami, zarysy budynków, świt i zmierzch.
4. W multiplayerze host i klienci powinni pobrać tę samą paczkę nightfix.

## Weryfikacja i ograniczenia

- Kompilacja edytora oraz gry: Succeeded. **128/128 testów** zaliczonych, bez błędów i pominiętych testów.
- Porównanie obrazu przed/po w Alderen o 22:00, dodatkowy test Norvak o 00:00: teren, wnętrze i pochodnia.
- Gotowy EXE z kontrolnie rozpakowanej paczki przeszedł ponowną kontrolę Alderen o 22:00 i zamknął się poprawnie, bez błędów ani zgłoszeń ensure w logu.
- W paczce publikacyjnej uaktualniono wyłącznie notatkę `POPRAWKA_NOCY.txt`; pliki wykonywalne i zasoby są tymi samymi, które przeszły powyższy test.
- ZIP: **1 833 214 618 bajtów (1,83 GB), 51 plików**; wszystkie kontrolnie rozpakowane i sprawdzone SHA-256. Bez nowych screenów, źródeł projektu i prywatnych zapisów.
- Nie przeprowadzono nowego testu WAN, wydajności 15 graczy ani renderu nocnego Sairen. Wspólne ustawienia dotyczą wszystkich regionów; pozostałe ograniczenia [bazowego 0.9.10](https://github.com/Aniosek/GearSoul-Playtest/releases/tag/v0.9.10) nadal obowiązują.

## Pobranie i uruchomienie

[Pobierz GearSoul — jaśniejsza noc, Windows](https://github.com/Aniosek/GearSoul-Playtest/releases/download/v0.9.10-nightfix/GearSoul_0.9.10_NightFix_Windows.zip).

Rozpakuj **cały ZIP do nowego folderu** i uruchom `GearlSoul1.exe` (Alderen) lub `START_GearSoul_Regiony.bat` (wybór regionu/hosta). Nie pobieraj „Source code” jako gry i nie uruchamiaj EXE wewnątrz ZIP-a. Zachowaj starsze zapisy; launchery testowe domyślnie wyłączają trwały zapis.

Numer bazowy w aplikacji i starszych instrukcjach pozostaje 0.9.10. Dokładne wydanie to **v0.9.10-nightfix**, zapisane też w `POPRAWKA_NOCY.txt`. Sumę pobrania znajdziesz w załączonym pliku SHA256 oraz w `SHA256SUMS.txt` repozytorium.

SHA-256 ZIP: `e39730775b170ff58ad1d94f51a70a1b879526554f382386cfdcb1a1172b64e8`.

Błędy: **gearsoul00@gmail.com** lub [GitHub Issues](https://github.com/Aniosek/GearSoul-Playtest/issues). Podaj wersję **0.9.10-nightfix**, region, godzinę w grze, host/klient oraz kroki odtworzenia. `CREATE_BUG_REPORT_PACKAGE.bat` przygotowuje pliki diagnostyczne; przejrzyj je przed wysłaniem, bo mogą zawierać adresy IP i nazwy katalogów.
