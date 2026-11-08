---
description: Wznawia pracę od najnowszego handoffu w session-logs/ (bez ładowania starej sesji).
---
Użyj skilla `session-handoff` w trybie **WZNOWIENIE**.

1. Znajdź **najnowszy** plik z frontmatterem `kind: handoff` w `session-logs/` (lub wskazany w $ARGUMENTS).
2. Przeczytaj **tylko ten plik**.
3. Sprawdź lekko stan faktyczny (`git status`, `git diff --stat`), czy handoff zgadza się z rzeczywistością.
4. Streść w ~3 liniach: **gdzie jesteśmy → następny krok → czego unikać** i poczekaj na potwierdzenie.
