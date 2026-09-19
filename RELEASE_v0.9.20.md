# GearSoul v0.9.20 — las, górskie kopalnie i praca w osadzie

**Rozwojowa pre-alpha. Etap 100 NIE jest ukończony. To NIE są beta testy ani wydanie 1.0.** Animacje, dalsze mechaniki i potwierdzona grywalność muszą zostać domknięte przed wejściem w betę. Numer wersji nie jest procentem ukończenia.

## Co dodano i poprawiono

- Las na wszystkich trzech mapach: 282 986 wcześniej dekoracyjnych drzew podłączono do ścinki, energii, zużycia narzędzi, praktyki i fizycznych kłód. Po zabraniu drewna miejsce można wykorzystać pod budowę, jeśli pozwalają na to podparcie, kolizje i prawa.
- Po dwie kopalnie w Alderen, Sairen i Norvak otoczono zamkniętymi skalnymi masywami z kolizją. Nadal wymagają wydobycia i przyniesionych podpór.
- 407 drzew zdjęto z odsłoniętej skały i przeniesiono na grunt wokół podnóży. Liczba drzew nie zmniejszyła się. Zachowano identyfikatory i obsługę wcześniejszego zapisu częściowej/pełnej wycinki.
- Budowane stanowisko kowalskie, dymarka i skrzynia magazynowa: własne dostawy materiałów, praca i działanie po ukończeniu.
- Wiadro wielokrotnego użytku, wytwarzane posłanie, siedzący odpoczynek i przestawianie ukończonych mebli gracza. Skrzynia mieści narzędzia oraz drobne materiały; przenosić można tylko pustą.
- Zapis cyklu sadzonki i drzewa, praktyka Barda oraz Myślistwa, odrębne pule do 50 Wiedzy i do 40 Rozwoju. Zachowano poprzednie poprawki nocnego światła, łowienie, pochodnie i rozmowę przestrzenną.

## Jak uruchomić i co testować

Pobierz `GearSoul_v0.9.20_PreAlpha_Multiplayer_Windows.zip`, rozpakuj **całość do nowego folderu** i uruchom `START_GearSoul_Regiony.bat` albo główne `GearlSoul1.exe`. EXE domyślnie otwiera Alderen. Nie uruchamiaj gry wewnątrz ZIP-a. Unreal Editor nie jest wymagany. Host i wszyscy klienci muszą mieć 0.9.20.

- Ścinanie także daleko od osady, miejsce po pniu i zgodność stanu u późno dołączającego gracza.
- Rozmieszczenie drzew przy skałach, drożne wejścia, wydobycie i fizyczne podpory kopalni.
- Budowa kuźni, dymarki, skrzyni i mebli, przenoszenie materiałów oraz brak ich powielania.
- Posłanie i odpoczynek, odzyskanie ruchu, przestawianie mebli, zawartość/limity skrzyni.
- Masa wody w wiadrze, napełnianie i zachowanie pustego pojemnika.
- Nadal barter, zaprzęg, jedzenie, ryby, nocne światło i głos na dwóch komputerach.

[Pełna instrukcja](https://github.com/Aniosek/GearSoul-Playtest/blob/main/README_PL.md) · [Checklista](https://github.com/Aniosek/GearSoul-Playtest/blob/main/TESTING_CHECKLIST_PL.md) · [Dalsza roadmapa](https://github.com/Aniosek/GearSoul-Playtest/blob/main/ROADMAP.md)

## Granice wersji

- Kopalnia to 6 odcinków / 12 m, nie dowolne kopanie całej góry, rozgałęzienia ani prawdziwe zawały.
- Drzewo znika po końcowym uderzeniu; brak animacji przewracania pnia. Nie odrasta automatycznie — sadzenie jest osobnym systemem.
- Odpoczynek jest na siedząco, nie pełną animacją snu. Animacje podejścia, niesienia i części prac oraz oprawa regionów nadal wymagają dopracowania.
- Domyślne launchery uruchamiają test bez trwałego zapisu. Nie kasuj wcześniejszych zapisów; nie jest to trwały serwer produkcyjny.
- Trzy mapy nie oznaczają gotowego transferu pomiędzy niezależnymi serwerami. W tej wersji nie potwierdzono WAN, wydajności 15 renderujących graczy ani wielodniowego masowego wyrębu.
- Do domknięcia pozostają dalsze wyposażenie produkcji/magazynów, gildie i rozwój osad, uzgodnione zasady offline oraz docelowa infrastruktura.

## Weryfikacja

- **143/143** testy regresji, bez błędów, ostrzeżeń testów i pominięć; obejmują zachowanie częściowej i pełnej wycinki po przeniesieniu drzewa.
- **142 Blueprinty**, bez błędów/ostrzeżeń ich kompilacji i nieudanych odczytów. Kompilacja edytora, gry, przygotowanie map i pakowanie zakończone powodzeniem. Zwykłe ostrzeżenia silnika nadal występują.
- Gotowy EXE: ścinka i zwolnienie kolizji po pniu na **3/3 mapach**, z renderowaniem obrazu. Obejrzano również oba skalne masywy każdego regionu; audyt rozmieszczenia wykazał 0 drzew na odsłoniętych nowych skałach i 0 przeniesionych drzew wewnątrz wykluczonego obszaru osad.
- Gotowy EXE: po jednej galerii na każdej z **3/3 map**, wydobycie sześciu odcinków, dostarczenie materiałów i ukończenie sześciu podpór, kontrola podłogi i miejsca dla postaci. To automatyczna próba bez renderowania, nie ręczne przejście każdej kopalni.
- Gotowy EXE: lokalny host, klient i późne dołączenie; cztery rzeczywiste sieciowe uderzenia, zgodne usunięcie drzewa. Próba z symulowanym opóźnieniem **100 ms i utratą 3% pakietów**, bez renderowania. Nie jest to test WAN ani wydajności 15 graczy.
- ZIP: **1 842 409 111 bajtów (1,84 GB), 50 plików**. Archiwum kontrolnie rozpakowano, a każdy plik porównano z paczką źródłową przez SHA-256. Testy powyżej wykonano na EXE z tego rozpakowania. Nie dołączono źródeł projektu ani jego kluczy szyfrowania.

SHA-256 pliku `GearSoul_v0.9.20_PreAlpha_Multiplayer_Windows.zip`:

```text
6c347e1719a27c410434d2cb5e4824e8c9f385f670f2a0c33882e6c5694b94bb
```

Te wyniki dotyczą opisanego zakresu, nie gwarantują braku wszystkich błędów ani finalnej jakości oprawy. Wydanie oznaczono jako **pre-release**; pobieraj załączony ZIP tej wersji, nie automatyczne „Source code” ani skrót „latest”, który może wskazywać starszą wersję.

## Zgłoszenia

**gearsoul00@gmail.com** lub [GitHub Issues](https://github.com/Aniosek/GearSoul-Playtest/issues). Podaj **0.9.20**, region, host/klient, kroki i oczekiwany rezultat. `CREATE_BUG_REPORT_PACKAGE.bat` pomaga zebrać diagnostykę. Przejrzyj ZIP przed wysłaniem — może zawierać IP, nazwy folderów i zapis świata.

Udostępniamy skompilowaną grę, nie źródła ani edytowalne modele. Starsze wydania pozostają dostępne. Do tego wydania nie dodano nowych publicznych screenshotów.
