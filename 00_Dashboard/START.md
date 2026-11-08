---
title: "START — panel główny inwestora"
typ: dokument
status: IN_PROGRESS
priorytet: CRITICAL
tagi: [#coordination]
updated: 2026-10-16
---

# START — panel główny inwestora

## Twierdzenia

Dashboard — bez własnych twierdzeń. Każda liczba poniżej ma ID twierdzenia, z którego pochodzi.

> **Dane demonstracyjne.** „Dom Przykładowy" jest w całości fikcyjny. Zastąp go swoją inwestycją (patrz [[docs/01_Szybki_Start]]).

## Inwestycja

**Dom Przykładowy** — budynek jednorodzinny z dachem płaskim, Zielonów Mały (fikcyjna miejscowość).
Etap: stan surowy otwarty, wybór wykonawcy dachu. Szybki stan: [[00_Dashboard/hot]].

## 🚨 Alerty (CRITICAL / HIGH)

| Alert | Priorytet | Termin |
|---|---|---|
| [[09_Ryzyka_i_Problemy/ALERTY/ALERT_Oferty_Dachu_Bez_Odwodnienia_Awaryjnego]] | HIGH | 2026-10-30 |

## ⚖️ Spory (`disputed`) do rozstrzygnięcia

| Temat | Twierdzenia | Rozstrzyga | Termin |
|---|---|---|---|
| Wysokość wywinięcia hydroizolacji na attyce | T-0006 vs T-0007 | projektantka | 2026-10-30 |

## 🧭 Decyzje w toku

| Decyzja | Status | Blokada |
|---|---|---|
| [[10_Decyzje/Hydroizolacja_Stropodachu_Decyzja]] | REVIEW | akceptacja drugiej inwestorki |

Pełna lista: [[10_Decyzje/Indeks_Decyzji]] · Ryzyka: [[09_Ryzyka_i_Problemy/Indeks_Ryzyk]]

## 💰 Dach — porównanie ofert

[[06_Budzet_i_Koszty/Oferty_Dach_Porownanie]] — znormalizowane ceny (T-0016) vs kosztorys (T-0014).

## 🧱 Punkty bez odwrotu

[[08_Harmonogram/Punkty_Bez_Odwrotu]] — następny: obróbki attyk (zablokowany sporem).

## 🔧 Operacje agenta

- Ostatni diff do przeglądu: [[_ops/diff-2026-10-15-ingest-oferty-dach]]
- Ostatni audyt LINT: [[17_Raporty/Audyty_Cykliczne/20261016_Audyt]]
- Rejestr źródeł: [[raw/RAW_INDEX]]
- Pytania otwarte: [[00_Dashboard/Otwarte_Pytania]]
