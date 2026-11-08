---
description: Zamyka etap budowy — zamraża stan faktyczny po punkcie bez odwrotu.
---
Punkt bez odwrotu: $ARGUMENTS

1. Wczytaj `08_Harmonogram/Punkty_Bez_Odwrotu.md` i znajdź pozycję.
2. Wypisz wszystkie twierdzenia opisujące stan objęty tym punktem.
3. Dla każdego zapytaj mnie: czy stan faktyczny zgadza się z twierdzeniem?
   Jeśli nie — poproś o źródło rangi 1 (zdjęcie z datą, wpis do dziennika,
   dokumentacja powykonawcza) i utwórz nowe twierdzenie, stare oznacz `superseded`.
4. Po potwierdzeniu wszystkich: ustaw `status: frozen`, `as-of` = data odbioru etapu.
5. Utwórz `13_Dziennik_Budowy/RRRR-MM-DD_Zamkniecie_[etap].md` z listą ID zamrożonych.
6. Zaktualizuj `Punkty_Bez_Odwrotu.md` i `00_Dashboard/hot.md`.

Zmiana klasy B — wyłącznie na gałęzi.
