---
name: session-handoff
description: Zapis i wznowienie pracy między sesjami bez ładowania całej poprzedniej rozmowy. Używaj, gdy użytkownik chce "zapisać handoff", "zamknąć sesję", "wznowić od ostatniej sesji", "przekazać kontekst" albo wpisuje /handoff lub /pickup.
---

# Session Handoff

Metoda **„udokumentuj i wyczyść"**: pod koniec sesji (gdy model jeszcze wszystko dobrze pamięta) zapisujesz **krótki, świadomie zredagowany plik**, a nową, czystą sesję zaczynasz od przeczytania **tylko tego pliku** — nie całej starej rozmowy.

Dlaczego to lepsze niż automatyczne `/compact`: kompaktowanie odpala się, gdy kontekst jest PEŁNY, i tworzy „streszczenia streszczeń". Handoff jest pisany świadomie, wcześniej, w jednym przebiegu.

## Dwa tryby

- **ZAPIS** (`/handoff`): zapisz lub zaktualizuj plik handoffu bieżącej sesji.
- **WZNOWIENIE** (`/pickup`): przeczytaj najnowszy handoff i wejdź w temat bez ładowania historii.

## Gdzie i jak nazywać

- Katalog: `session-logs/` w katalogu głównym (utwórz, jeśli brak). Katalog jest w `.gitignore`.
- Nazwa: `RRRR-MM-DD-slug.md`, slug = 2-4 słowa o temacie sesji.
- Jeśli **dzisiejszy plik na ten sam temat** istnieje — **zaktualizuj go**.
- Handoffy rozpoznaje się po frontmatterze `kind: handoff`.

## Format pliku

```markdown
---
kind: handoff
date: RRRR-MM-DD
topic: <slug>
status: in-progress | done | blocked
---

# <Jedno zdanie: o czym była sesja>

## Podsumowanie
2-4 zdania: co zrobiliśmy i dlaczego.

## Kluczowe ustalenia
- ustalenie + **dlaczego**

## Stan
- ✅ zrobione: ...
- 🔄 w toku: ...
- ⛔ zablokowane / czekamy na: ...

## Artefakty
- ścieżki plików, gałąź, diff w `_ops/`

## Następny krok
Jeden konkretny ruch, od którego zaczyna nowa sesja.

## Czego NIE robić
Ślepe uliczki i odrzucone podejścia.
```

## Reguły treści

- **Nigdy nie zapisuj sekretów ani danych osobowych** (hasła, tokeny, PESEL, numery kont). Odwołuj się do miejsca, nie kopiuj wartości.
- **Nie duplikuj artefaktów** (diffy, decyzje, commity) — linkuj do nich.
- **Handoff to nie wiedza o budowie.** Każdy nowy fakt o inwestycji musi trafić do bazy jako twierdzenie ze źródłem (np. notatka w `raw/korespondencja/` + INGEST). Handoff przepada po zamknięciu wątku.

## Kiedy zapisywać

- Przy ~50-60% zużycia kontekstu, nie przy 90%.
- Przy zamknięciu wątku, przed zmianą zadania, na koniec dnia.

## WZNOWIENIE (/pickup)

1. Znajdź najnowszy plik z `kind: handoff` w `session-logs/`.
2. Przeczytaj tylko ten plik.
3. Sprawdź stan: `git status`, `git diff --stat`, aktualna gałąź.
4. Streść w ~3 liniach: **gdzie jesteśmy → następny krok → czego unikać**. Poczekaj na potwierdzenie.
