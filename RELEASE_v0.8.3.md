# GearSoul v0.8.3 — dom średniowieczny budowany etapami

Pierwszy dom z dwiema izbami, ciosanym szkieletem, glinianymi ścianami, podmurówką i gontem jest na mapie. Obok jest plac do własnej budowy, skrzynia ze skończonym zapasem materiałów oraz stanowisko do kucia gwoździ.

## Jak przetestować

1. Pobierz ZIP załączony poniżej i rozpakuj go w całości. Nie pobieraj „Source code” — to tylko dokumentacja repozytorium.
2. Uruchom `START_GearSoul_Solo.bat` lub `START_GearSoul_Host.bat`; drugi gracz używa `START_GearSoul_Join.bat`.
3. Sprawdź gotowy dom: wejście, dwie izby, stół, ławy, łóżko, skrzynię i ochronę przed pogodą.
4. Zbuduj drugi dom, donosząc pojedyncze materiały. Łącznie potrzeba 6 kamieni, 14 kłód, 8 gliny, 18 gwoździ oraz 54 cykli pracy. Wymagany jest poziom 1 ciesielstwa, przydzielony punkt wiedzy, sprawny młotek i narzędzie wskazane przy etapie.
5. Sprawdź wspólny postęp z drugim budowniczym, odmowę użycia złego materiału/narzędzia, zużycie energii i poprawny powrót do ruchu.

Szczegółowa instrukcja `README_PL.md` jest w paczce oraz repozytorium. Zgłoszenia: **gearsoul00@gmail.com** lub GitHub Issues. `CREATE_BUG_REPORT_PACKAGE.bat` pomaga zebrać logi — przejrzyj paczkę przed jej wysłaniem.

## Zweryfikowane przed publikacją

- 80/80 testów automatycznych; kompilacja i przygotowanie danych gry zakończone powodzeniem.
- Pełna budowa przez rzeczywiste interakcje w gotowym EXE: 8 etapów, 54 cykle pracy.
- Test mapy z serwerem i dwoma klientami z ponownie rozpakowanego ZIP-a: zaliczony, obie postacie animowane, brak błędów krytycznych.
- 57 plików w ZIP-ie, każdy sprawdzony SHA-256 po rozpakowaniu. Rozmiar: 1 566 990 172 bajty.

## Uczciwie o ograniczeniach

To pre-alpha. Meble i otwarte drzwi są na razie statyczne. Ruch narzędzia to proceduralna animacja ręki, nie osobna choreografia każdego gwoździa. Odtwarzanie nowo zbudowanych domów po pełnym restarcie świata nie jest ukończone. Nie przeprowadzono nowego testu WAN ani profilu 15 graczy dla tej wersji.

Paczka zawiera skompilowaną grę i ugotowane zasoby, bez kodu, PDB ani źródłowych modeli MetaHuman.

![Dom w grze](https://raw.githubusercontent.com/Aniosek/GearSoul-Playtest/main/screenshots/v0.8.3/01_dom_w_grze.png)

![Budowa w grze](https://raw.githubusercontent.com/Aniosek/GearSoul-Playtest/main/screenshots/v0.8.3/02_budowa_w_grze.png)
