# GearSoul v0.8.1 — odzież, moknięcie i ochrona przed pogodą

Publiczna wersja pre-alpha do testów multiplayerowych Etapów 0–71.

## Najważniejsze zmiany

- trzy fizyczne warstwy odzieży: bazowa, ocieplająca i zewnętrzna,
- lniana koszula spodnia, wełniana tunika i skórzany płaszcz z własnym GUID-em, masą, objętością, jakością, trwałością oraz wilgotnością,
- moknięcie podczas burzy od warstwy zewnętrznej do wewnętrznej,
- niższa izolacja przemoczonych ubrań oraz ochrona ograniczająca, ale nigdy całkowicie wyłączająca wpływ temperatury,
- naturalne suszenie i suszenie do sześciu razy szybsze przy rozpalonym ognisku,
- atomowa zamiana ubrania w tej samej warstwie bez utraty przedmiotu oraz niezależne wyposażenie plecaka,
- wersjonowany zapis schematu 3 zachowujący wilgotność każdej fizycznej sztuki odzieży,
- polskie opisy, informacje o warstwach i wilgotności oraz sześć pickupów na mapie testowej.

Warstwy działają mechanicznie i są widoczne w interfejsie. Widoczna zmiana stroju MetaHumana nie jest jeszcze częścią tej wersji; modele ubrań leżących na ziemi pozostają prototypowe.

## Weryfikacja

- build edytora Unreal Engine 5.8: sukces,
- automatyzacja: 75/75 testów zakończonych sukcesem,
- pełna regresja multiplayer: serwer, dwóch klientów, bezpieczeństwo i medycyna — sukces,
- restart trwałego zapisu: sekwencja `0→1→2` zachowana,
- końcowy `BuildCookRun`: `BUILD SUCCESSFUL`, kod 0,
- smoke test finalnego EXE: trzy warstwy, moknięcie, suszenie, zlecenia, pożyczki i dwóch klientów — sukces,
- pełny odczyt 73 plików archiwum ZIP: bez błędu,
- paczka nie zawiera PDB, kodu źródłowego, zapisów gry ani edytowalnych źródeł MetaHumana.

## Instalacja

1. Pobierz ZIP i rozpakuj go w całości.
2. Wejdź do folderu `Windows`.
3. Uruchom `START_GearSoul_Solo.bat`, `START_GearSoul_Host.bat` albo `START_GearSoul_Join.bat`.
4. Nie uruchamiaj EXE bezpośrednio z wnętrza archiwum.

SHA-256:

```text
29783DDC42B03B93C871C375FAC4CAF471860C7C0A6D5D87E758A04EC6110781
```
