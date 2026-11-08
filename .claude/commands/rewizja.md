---
description: Wprowadza nową rewizję dokumentu projektowego i wykrywa rozjazdy z bazą.
---
Nowa rewizja: $ARGUMENTS

1. Wpisz do `raw/RAW_INDEX.md`, poprzednią rewizję → `ZASTĄPIONY`.
2. Znajdź WSZYSTKIE twierdzenia cytujące poprzednią rewizję → `stale`.
3. Porównaj nową rewizję ze starą. Wypisz różnice w trzech grupach:
   - zmiany niekolidujące z niczym,
   - zmiany kolidujące z twierdzeniami `active`,
   - **zmiany kolidujące z twierdzeniami `frozen`** ← ALERT, nie aktualizacja.
4. Dla grupy 3 utwórz `09_Ryzyka_i_Problemy/ALERTY/ALERT_Rozjazd_Projekt_vs_Stan_Faktyczny_[temat].md`.
5. Nie przepisuj twierdzeń `stale` — to osobna sesja weryfikacyjna.
6. Wygeneruj diff i zatrzymaj się.
