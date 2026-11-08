---
title: "Porównanie ofert — hydroizolacja stropodachu"
typ: budzet
status: IN_PROGRESS
priorytet: HIGH
tagi: [#cost, #decision, #construction]
updated: 2026-10-16
---

# Porównanie ofert — hydroizolacja stropodachu

## Twierdzenia

- [T-0010] {status: active} {pewność: FAKT} {as-of: 2026-09-10} {ważne-do: 2026-11-10} {wymaga: —}
  Dachy Alfa zaoferowały membranę EPDM 1,2 mm na 172 m² wraz z ociepleniem, obróbkami attyk oraz 4 wpustami i 2 przelewami awaryjnymi, a pozycje oferty sumują się do 61 400 zł netto.
  Źródło: [[raw/oferty/dach/2026-09-10_Dachy_Alfa_oferta.md]] (S-003) poz. 1–4 | ranga: 6

- [T-0011] {status: active} {pewność: FAKT} {as-of: 2026-09-10} {ważne-do: 2026-11-10} {wymaga: —}
  W ofercie Dachy Alfa pole „Razem netto" podaje 58 400 zł, czyli o 3 000 zł mniej niż suma pozycji.
  Źródło: [[raw/oferty/dach/2026-09-10_Dachy_Alfa_oferta.md]] (S-003) | ranga: 6

- [T-0012] {status: active} {pewność: FAKT} {as-of: 2026-09-14} {ważne-do: 2026-11-14} {wymaga: —}
  Izolbud Beta zaoferował ryczałtowo papę termozgrzewalną dwuwarstwową na 190 m² z ociepleniem i 4 wpustami za 52 900 zł netto, bez obróbek attyk i bez przelewów awaryjnych.
  Źródło: [[raw/oferty/dach/2026-09-14_Izolbud_Beta_oferta.md]] (S-004) | ranga: 6

- [T-0013] {status: stale} {pewność: FAKT} {as-of: 2026-09-18} {ważne-do: 2026-10-12} {wymaga: —}
  Membrana Gamma zaoferowała membranę PVC 1,5 mm na 172 m² z ociepleniem, obróbkami attyk i 4 wpustami (bez przelewów awaryjnych) za 49 800 zł netto.
  Źródło: [[raw/oferty/dach/2026-09-18_Membrana_Gamma_oferta.md]] (S-005) | ranga: 6
  Status stale: oferta wygasła 2026-10-12 (LINT 2026-10-16) — cena tylko poglądowa.

- [T-0014] {status: active} {pewność: HIPOTEZA} {as-of: 2026-09-05} {ważne-do: 2026-12-05} {wymaga: —}
  Kosztorys inwestorski wycenia pełny zakres stropodachu wg PT rev.1 na 56 000 zł netto.
  Źródło: [[raw/kosztorysy/Kosztorys_inwestorski_dach.md]] (S-010) | ranga: 7

- [T-0015] {status: active} {pewność: REKOMENDACJA} {as-of: 2026-10-15} {ważne-do: PT-rev-next} {wymaga: —}
  Powierzchnia w ofercie Izolbud Beta jest o 18 m² (ok. 10%) większa od powierzchni projektowej.
  Wyprowadzone z: T-0003, T-0012 | ranga: 8

- [T-0016] {status: active} {pewność: REKOMENDACJA} {as-of: 2026-10-15} {ważne-do: 2026-11-10} {wymaga: akceptacja-inwestorów}
  Po sprowadzeniu do wspólnego zakresu PT rev.1 oferty kosztują netto: Dachy Alfa 61 400 zł, Izolbud Beta 57 200–62 200 zł, Membrana Gamma 50 900 zł (wygasła).
  Wyprowadzone z: T-0010, T-0012, T-0013, T-0015 (stawki brakujących pozycji przyjęte z oferty Dachy Alfa) | ranga: 8

- [T-0017] {status: active} {pewność: REKOMENDACJA} {as-of: 2026-10-15} {ważne-do: 2026-11-10} {wymaga: —}
  Względem kosztorysu inwestorskiego znormalizowane oferty odchylają się o: Dachy Alfa +9,6%, Izolbud Beta od +2% do +11%, Membrana Gamma −9%.
  Wyprowadzone z: T-0014, T-0016 | ranga: 8

## Matryca porównawcza (zakres wspólny = PT rev.1)

| Pozycja | Dachy Alfa | Izolbud Beta | Membrana Gamma |
|---|---|---|---|
| Technologia | EPDM 1,2 mm | papa 2-warstwowa | PVC 1,5 mm |
| Powierzchnia w ofercie | 172 m² ✅ | 190 m² ⚠️ (T-0015) | 172 m² ✅ |
| Obróbki attyk | ✅ | ❌ dolicz 8 200 | ✅ |
| Przelewy awaryjne (2 szt.) | ✅ | ❌ dolicz 1 100 | ❌ dolicz 1 100 |
| Cena w ofercie | 58 400 ⚠️ błąd sumy (T-0011) | 52 900 | 49 800 |
| **Cena znormalizowana** | **61 400** | **57 200–62 200** | **50 900** |
| vs kosztorys 56 000 | +9,6% | +2% … +11% | −9% |
| Ważność | do 2026-11-10 | do 2026-11-14 | **wygasła** |

Widełki Izolbud Beta: górna = ryczałt + brakujące pozycje; dolna = jw. minus proporcjonalna korekta za 18 m² nadwyżki powierzchni (ok. 5 000 zł). Wszystkie kwoty netto, zł.

## Kontekst

Matryca powstała w ingeście z [[_ops/diff-2026-10-15-ingest-oferty-dach]]. Parametry projektowe — [[03_Projekt/Architektura/Stropodach]]. Brak przelewów awaryjnych w dwóch ofertach → [[09_Ryzyka_i_Problemy/Ryzyka_Miedzybranzowe/Odwodnienie_Awaryjne_Stropodachu]]. Wybór — [[10_Decyzje/Hydroizolacja_Stropodachu_Decyzja]]. Streszczenia ofert: [[15_Knowledge_Base/2026-09-10_Dachy_Alfa_oferta]], [[15_Knowledge_Base/2026-09-14_Izolbud_Beta_oferta]], [[15_Knowledge_Base/2026-09-18_Membrana_Gamma_oferta]].

## Pytania do oferentów

- Dachy Alfa: która kwota wiąże — suma pozycji czy pole „Razem"?
- Izolbud Beta: skąd 190 m²? Prośba o rozbicie ryczałtu i wycenę obróbek oraz przelewów.
