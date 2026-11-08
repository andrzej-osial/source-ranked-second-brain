---
title: "Diff 2026-10-15 — ingest ofert na stropodach (demo)"
typ: dokument
status: REVIEW
priorytet: HIGH
tagi: [#cost, #construction]
updated: 2026-10-15
---

# Diff 2026-10-15 — ingest ofert na stropodach

## Twierdzenia

Plik operacyjny — bez własnych twierdzeń. Gałąź: `agent/2026-10-15-ingest-oferty-dach`. **NIE scalać do main przed `/diff-review`.**

## Lista twierdzeń przedstawiona inwestorowi PRZED zapisem

T-0010…T-0017 (oferty i normalizacja), T-0020 (ryzyko), T-0025 (decyzja), T-0006/T-0007 (spór o wywinięcie), T-0009 (UNVERIFIED). Zaakceptowane w sesji 2026-10-15, z jedną zmianą: T-0016 dostał `wymaga: akceptacja-inwestorów`.

## Klasa A (zapisane od razu)

| Zmiana | Plik |
|---|---|
| S-003, S-004, S-005, S-006, S-010, S-011 dopisane | [[raw/RAW_INDEX]] |
| 3 streszczenia 1:1 | [[15_Knowledge_Base/2026-09-10_Dachy_Alfa_oferta]], [[15_Knowledge_Base/2026-09-14_Izolbud_Beta_oferta]], [[15_Knowledge_Base/2026-09-18_Membrana_Gamma_oferta]] |
| T-0006, T-0007, T-0009 (nowe, bez konfliktu z istniejącymi) | [[03_Projekt/Architektura/Stropodach]] |
| T-0020 + alert HIGH | [[09_Ryzyka_i_Problemy/Ryzyka_Miedzybranzowe/Odwodnienie_Awaryjne_Stropodachu]], [[09_Ryzyka_i_Problemy/ALERTY/ALERT_Oferty_Dachu_Bez_Odwodnienia_Awaryjnego]] |
| T-0025 + karta decyzji (status REVIEW) | [[10_Decyzje/Hydroizolacja_Stropodachu_Decyzja]] |
| CHANGELOG, hot.md, START.md, indeksy | — |

## Klasa B (na gałęzi — do decyzji)

### Supersession

| Przegrywa | Wygrywa | Powód |
|---|---|---|
| T-0001 (ocieplenie 20 cm, notatka ze spotkania, **ranga 7**) | T-0004 (ocieplenie 25 cm, PT rev.1, **ranga 3**) | wyższa ranga wygrywa (reguła 1) |

### Zmiany w `06_Budzet_i_Koszty/`

| Zmiana | Plik |
|---|---|
| T-0010…T-0017 + matryca porównawcza | [[06_Budzet_i_Koszty/Oferty_Dach_Porownanie]] |

### Propozycja statusu FINAL

| Decyzja | Propozycja | Blokada |
|---|---|---|
| [[10_Decyzje/Hydroizolacja_Stropodachu_Decyzja]] | FINAL — wariant A po korekcie sumy | brak akceptacji drugiej inwestorki |

## DECYZJA CZŁOWIEKA WYMAGANA

1. **`disputed` T-0006 vs T-0007** — wysokość wywinięcia na attyce (15 cm vs 10 cm). Równa ranga (7), ta sama data. Rozstrzyga: **projektantka**. Termin: **2026-10-30**.
2. **Błąd sumy w ofercie Dachy Alfa** (T-0011) — która kwota wiąże? ➜ zapytanie do oferenta.
3. **Powierzchnia 190 m² w ofercie Izolbud Beta** (T-0015) ➜ zapytanie do oferenta.
4. **Akceptacja drugiej inwestorki** dla karty decyzji.

## Komenda merge (po akceptacji wszystkich pozycji)

```
git checkout main
git merge --no-ff agent/2026-10-15-ingest-oferty-dach
```
