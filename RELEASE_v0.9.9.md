# GearSoul v0.9.9 — trzy regiony, budowanie i czat głosowy

Wydanie Windows Pre-Alpha. **Nie jest to ukończone 1.0.0 ani deklaracja 99% gotowości.**

## Nowe w paczce

- Alderen, Sairen i Norvak, każdy z terenem, osadą, pięcioma wariantami domów i regionalną fauną. Alderen jest mapą domyślną; stara plansza pozostaje osobnym dodatkiem testowym.
- Panel **F10**: mikrofon, słuchawki/głośniki, lokalny odsłuch i miernik sygnału, głośność rozmowy oraz odtwarzanie w nieaktywnym oknie.
- Rozmowa na 25 m: obaj gracze włączają głos, zamykają menu, mówiący trzyma V. Dwa okna na jednym komputerze wymagają dźwięku w tle u odbiorcy. Mikrofon nie uruchamia się przy samym otwarciu ustawień.
- Budowanie z fizycznymi dostawami, noszenie kłód, profil i osobne budżety wiedzy/rozwoju.
- Prototyp kopalni: trzeba przebić skałę i budować podpory z przynoszonych kłód. Brak gotowego, otwartego korytarza na starcie.

## Uruchomienie

Pobierz **GearSoul_v0.9.9_PreAlpha_Multiplayer_Windows.zip** z załączników tego wydania i rozpakuj całość. „Source code” nie zawiera gry. Unreal Editor nie jest potrzebny.

`START_GearSoul_Regiony.bat` wybiera region oraz solo/host. `START_GearSoul_Join.bat` łączy się z adresem hosta. Zwykły EXE startuje w Alderen. Launchery testowe nie utrwalają świata. Dla Internetu nadal potrzebne jest połączenie do hosta na UDP 7777.

W F10 najpierw wybierz prawdziwy mikrofon i słuchawki. Test mikrofonu trwa do 15 s, nie zapisuje nagrania i nie wysyła go innym graczom. Używaj słuchawek — nie ma automatycznego usuwania echa głośników.

## Sprawdzone przed publikacją

- Regresja projektu: 126/126 testów, 0 błędów.
- Audio: enumeracja urządzeń, zmiana wyjścia, pobieranie próbek testowego tonu przez rzeczywisty mikser audio, przywrócenie sterowania po zamknięciu ustawień.
- Serwer + dwaj renderujący klienci oraz osobno listen-host + klient: 100 ms opóźnienia i 3% strat, pięć faz zasięgu/wyciszenia/zgody, uruchomione odtwarzanie.
- Test gotowego EXE potwierdził start w **Alderen bez podawania mapy**, panel audio i odtwarzanie tonu. Ten sam EXE przeszedł test głosu listen-host + klient.
- Wszystkie trzy mapy w gotowym EXE: po 20 domów / 5 wariantów, 900 kontroli dachów i 20 przejść przez drzwi na region — bez błędów. Fauna: 38 / 42 / 30; próba ruchu przeszła w każdym regionie.
- Wydobycie w gotowym EXE na Alderen: 90 czynności, 6 ukończonych podpór i wyczerpanie złoża bez zniknięcia podłoża wyrobiska.
- Po kontrolnym rozpakowaniu ZIP-a uruchomiono jego główne EXE: start w Alderen, wykrycie urządzeń, odtwarzanie tonu oraz zamknięcie ustawień z odzyskaniem ruchu — wynik pozytywny.

Automatyczne próby głosu używają sygnału syntetycznego — nie zastępują rozmowy dwóch ludzi na fizycznych mikrofonach. Prosimy sprawdzić to na własnym sprzęcie.

## Kontrola archiwum

ZIP ma **1,82 GB (1 821 948 486 bajtów)** i 54 pliki. Archiwum rozpakowano kontrolnie; każdy plik jest identyczny z przygotowaną paczką według SHA-256. W środku są pliki wykonywalne, ugotowana zawartość, launchery, instrukcja i cztery screeny. Nie zawiera projektu źródłowego, zapisów testerów ani ich logów.

SHA-256 ZIP-a: `a3e0b00070e3a920ca4490c51cd5db01b289b549854cc23f6728b272c2abed4c`.

## Znane ograniczenia

- Kopalnie: sześć odcinków / 12 m, brak swobodnych rozgałęzień i prawdziwych zawałów; wnętrze wymaga jeszcze oświetlenia. Podpory blokują dalszą pracę, ale nie symulują konstrukcji geotechnicznej.
- Regiony są pierwszą wersją terenu i oprawy. Część lasu jest dekoracyjna, oświetlenie i optymalizacja pozostają do dopracowania.
- Meble nie mają jeszcze wszystkich interakcji; nie ma kompletnego łańcucha budowy każdego warsztatu od zera.
- Regiony nie są połączone działającym transferem między niezależnymi serwerami. Launchery uruchamiają świeży świat testowy, nie produkcyjny serwer trwały.
- Nie potwierdzono wydajności 15 renderujących klientów ani testów połączeń WAN dla tego wydania.

Instrukcja: [README_PL.md](https://github.com/Aniosek/GearSoul-Playtest/blob/main/README_PL.md). Błędy: **gearsoul00@gmail.com** lub GitHub Issues. Dołącz wersję, region, host/klient, urządzenia audio i kroki odtworzenia. Przed wysłaniem paczki diagnostycznej przejrzyj logi i zapis pod kątem prywatnych danych.
