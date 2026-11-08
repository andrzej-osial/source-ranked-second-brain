---
title: "QUERY — która oferta na dach jest najkorzystniejsza? (przykład odpowiedzi)"
typ: analiza
status: FINAL
priorytet: MEDIUM
tagi: [#cost, #decision]
updated: 2026-10-16
---

# QUERY: która oferta na dach jest najkorzystniejsza?

## Twierdzenia

- [T-0050] {status: active} {pewność: REKOMENDACJA} {as-of: 2026-10-16} {ważne-do: 2026-11-10} {wymaga: akceptacja-inwestorów}
  Najpełniej udokumentowaną i zgodną z projektem ofertą jest Dachy Alfa, pod warunkiem wyjaśnienia błędu sumy.
  Wyprowadzone z: T-0005, T-0010, T-0011, T-0016 | ranga: 8

## Kontekst

Przykład odpowiedzi w trybie `/query` — pokazuje obowiązkową strukturę. Synteza zapisana tu, bo jest cenna; jako analiza AI ma rangę 8 i **nie może być źródłem FAKT**. Powiązane: [[06_Budzet_i_Koszty/Oferty_Dach_Porownanie]].

## OSTRZEŻENIA

- Oferta Membrana Gamma wygasła — jej cena jest tylko poglądowa (T-0013, `stale`).
- Wysokość wywinięcia na attyce jest sporna (T-0006, T-0007, `disputed`) — może zmienić zakres każdej oferty.
- Wysokość attyki nie jest potwierdzona (T-0009, `UNVERIFIED`).
- Ceny znormalizowane to wyliczenia, nie fakty (T-0016, ranga 8).

## ODPOWIEDŹ

- Projekt wymaga 4 wpustów i 2 przelewów awaryjnych (T-0005).
- Tylko Dachy Alfa wyceniły pełny zakres z projektu (T-0010), ale ich pole „Razem" zaniża sumę o 3 000 zł (T-0011).
- Izolbud Beta liczy 190 m² zamiast 172 m² (T-0015) i nie wycenia obróbek ani przelewów (T-0012).
- Po normalizacji: Alfa 61 400 zł, Beta 57 200–62 200 zł (T-0016); kosztorys inwestorski to 56 000 zł (T-0014).
- Do negocjacji przeszły Alfa i Beta (T-0025).

## LUKI

- Pisemne wyjaśnienie Dachy Alfa, która kwota wiąże.
- Rozbicie ryczałtu Izolbud Beta i źródło powierzchni 190 m².
- Pisemne stanowisko projektantki w sprawie wysokości wywinięcia i attyki (rozstrzygnie T-0006/T-0007 i T-0009).

## PYTANIA KONTROLNE (inspektor nadzoru)

1. Czy zakres umowy obejmuje przelewy awaryjne zgodnie z PT rev.1?
2. Na jakiej wysokości kończy się hydroizolacja na attyce i kto to zatwierdził na piśmie?
3. Czy powierzchnia rozliczeniowa w umowie odpowiada 172 m² z projektu?
