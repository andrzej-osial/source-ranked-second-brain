---
title: "RAW INDEX — rejestr źródeł"
typ: dokument
status: IN_PROGRESS
priorytet: HIGH
tagi: []
updated: 2026-10-16
---

# RAW INDEX — rejestr źródeł

## Twierdzenia

Rejestr operacyjny — bez własnych twierdzeń. Każdy plik w `raw/` ma tu wiersz, zanim zostanie użyty jako źródło.

**Zasada:** folder `raw/` jest tylko do odczytu. Streszczenie 1:1 trafia do `15_Knowledge_Base/`, a twierdzenia atomowe do katalogów docelowych wg reguł routowania z [[CLAUDE]].

> Wszystkie wpisy poniżej to **fikcyjne dane demonstracyjne** („Dom Przykładowy").

## Statusy źródeł

| Status | Znaczenie |
|---|---|
| AKTUALNY | Obowiązująca wersja dokumentu |
| ZASTĄPIONY | Jest nowsza rewizja — twierdzenia cytujące ten dokument → `stale` |
| WYGASŁY | Minęła data ważności (oferty) — twierdzenia → `stale` |
| ARCHIWALNY | Zachowany dla historii, nieużywany |

## Rejestr

| ID | Plik | Typ | Ranga | Rewizja | Data dok. | Ważne do | Status | Zastępuje |
|---|---|---|---|---|---|---|---|---|
| S-001 | [[raw/projekt/PAB_Dom_Przykladowy.md]] | projekt budowlany | 4 | rev.0 | 2026-03-02 | — | AKTUALNY | — |
| S-002 | [[raw/projekt/PT_Stropodach_rev1.md]] | projekt techniczny | 3 | PT rev.1 | 2026-08-20 | — | AKTUALNY | S-009 |
| S-003 | [[raw/oferty/dach/2026-09-10_Dachy_Alfa_oferta.md]] | oferta | 6 | — | 2026-09-10 | 2026-11-10 | AKTUALNY | — |
| S-004 | [[raw/oferty/dach/2026-09-14_Izolbud_Beta_oferta.md]] | oferta | 6 | — | 2026-09-14 | 2026-11-14 | AKTUALNY | — |
| S-005 | [[raw/oferty/dach/2026-09-18_Membrana_Gamma_oferta.md]] | oferta | 6 | — | 2026-09-18 | 2026-10-12 | WYGASŁY | — |
| S-006 | [[raw/korespondencja/2026-09-20_notatka_spotkanie_dach.md]] | notatka ze spotkania | 7 | — | 2026-09-20 | — | AKTUALNY | — |
| S-007 | [[raw/korespondencja/2026-07-02_notatka_spotkanie_budowa.md]] | notatka ze spotkania | 7 | — | 2026-07-02 | — | AKTUALNY | — |
| S-008 | [[raw/zdjecia/2026-08-28_strop_betonowanie.md]] | zdjęcia z datą | 1 | — | 2026-08-28 | — | AKTUALNY | — |
| S-009 | [[raw/projekt/PT_Stropodach_rev0.md]] | projekt techniczny | 3 | PT rev.0 | 2026-06-10 | — | ZASTĄPIONY | — |
| S-010 | [[raw/kosztorysy/Kosztorys_inwestorski_dach.md]] | kosztorys (korespondencja) | 7 | — | 2026-09-05 | — | AKTUALNY | — |
| S-011 | [[raw/korespondencja/2026-10-14_notatka_decyzja_inwestora.md]] | notatka decydenta | 7 | — | 2026-10-14 | — | AKTUALNY | — |
| S-012 | [[raw/artykuly/Poradnik_hydroizolacje_dachow_plaskich.md]] | artykuł (notatka z lektury) | 8 | — | 2026-10-01 | — | AKTUALNY | — |

## Historia zmian rejestru

| Data | Zmiana |
|---|---|
| 2026-08-21 | S-002 (PT rev.1) wprowadzony → S-009 `ZASTĄPIONY`, T-0008 → `stale` |
| 2026-10-16 | LINT: S-005 po dacie ważności → `WYGASŁY`, T-0013 → `stale` |
