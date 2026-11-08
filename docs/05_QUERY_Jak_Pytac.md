# Jak zadać pytanie (QUERY)

```
/query Czy możemy podpisać umowę na dach z wybranym wykonawcą?
```

## Co robi agent

1. Czyta `00_Dashboard/hot.md` → `START.md` → indeksy → dopiero pliki szczegółowe.
2. Używa **wyłącznie** twierdzeń `active` i `frozen`.
3. Każde zdanie odpowiedzi ma ID twierdzenia, np. `(T-0010)`.
4. Nie uzupełnia luk wiedzą ogólną modelu. Czego nie ma w twierdzeniach — tego „nie wie".

## Obowiązkowa struktura odpowiedzi

| Sekcja | Po co |
|---|---|
| **OSTRZEŻENIA** | na początku: `stale`, `disputed`, `UNVERIFIED`, wygasłe oferty, zastąpione rewizje |
| **ODPOWIEDŹ** | zdania z ID |
| **LUKI** | jakiego konkretnego dokumentu brakuje |
| **PYTANIA KONTROLNE** | 2-3 pytania, które zadałby inspektor nadzoru |

Tryb jest **adwersaryjny**: odpowiedź ma przetrwać pytania drugiego inwestora albo inspektora.

## Dobre pytania

- „Co blokuje następny punkt bez odwrotu?"
- „Które oferty wygasną w ciągu 14 dni?"
- „Czy zakres oferty X pokrywa projekt techniczny? Wypisz brakujące pozycje."
- „Jakie twierdzenia opierają się tylko na ustaleniach ustnych?"

## Zapisywanie odpowiedzi

Cenną syntezę agent zapisuje w `14_AI_Analizy/rrrrmmdd_Temat.md` z twierdzeniami rangi 8. Przykład: [[14_AI_Analizy/20261016_Ktora_Oferta_Dachu]].
