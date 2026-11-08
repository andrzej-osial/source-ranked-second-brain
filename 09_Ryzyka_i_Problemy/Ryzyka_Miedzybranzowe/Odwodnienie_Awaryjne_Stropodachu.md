---
title: "Ryzyko — oferty dachu bez odwodnienia awaryjnego"
typ: ryzyko
status: OPEN
priorytet: HIGH
prawdopodobienstwo: HIGH
wplyw: HIGH
obszar: konstrukcja
wlasciciel: Jan Przykładowy (inwestor)
deadline: 2026-10-30
tagi: [#risk, #construction, #coordination]
updated: 2026-10-15
---

# Ryzyko — oferty dachu bez odwodnienia awaryjnego

## Twierdzenia

- [T-0020] {status: active} {pewność: REKOMENDACJA} {as-of: 2026-10-15} {ważne-do: PT-rev-next} {wymaga: akceptacja-inwestorów}
  Dwie z trzech ofert na stropodach nie obejmują 2 przelewów awaryjnych wymaganych w projekcie technicznym.
  Wyprowadzone z: T-0005, T-0012, T-0013 | ranga: 8

## Opis ryzyka

Jeśli umowa zostanie podpisana na zakres z oferty bez przelewów awaryjnych, dach zostanie wykonany niezgodnie z projektem technicznym. Przy zatkanym wpuście woda nie ma drogi ucieczki — zalega na dachu i obciąża konstrukcję lub przecieka przez obróbki attyk.

Ryzyko międzybranżowe: dotyka architektury (attyka), konstrukcji (obciążenie wodą) i budżetu (dopłata po podpisaniu umowy).

## Skutek (jeśli się zmaterializuje)

- dopłata za przeróbki attyki po wykonaniu obróbek,
- spór z wykonawcą o zakres umowy,
- ryzyko zalania przy intensywnym deszczu.

## Ocena

| Parametr | Ocena | Uzasadnienie |
|---|---|---|
| Prawdopodobieństwo | HIGH | 2 z 3 ofert pomijają pozycję (T-0020) |
| Wpływ | HIGH | niezgodność z projektem, ryzyko zalania |
| Priorytet | HIGH | → alert |

## Sygnały ostrzegawcze

1. Projekt umowy bez pozycji „przelewy awaryjne".
2. Wykonawca proponuje „zastępczo" większą liczbę zwykłych wpustów.

## Działania zapobiegawcze

- [ ] Wpisać przelewy awaryjne jako obowiązkową pozycję w zapytaniu doprecyzowującym — inwestor / 2026-10-20
- [ ] Wymagać pozycji w każdym projekcie umowy (checklista przed podpisaniem) — inwestor / przed podpisaniem
- [ ] Potwierdzić u projektantki lokalizację przelewów po zmianie attyki w PT rev.1 — inwestor / 2026-10-30

## Plan awaryjny

1. Aneks do umowy z wyceną przelewów przed wykonaniem obróbek attyk.

## Powiązane

- Alert: [[09_Ryzyka_i_Problemy/ALERTY/ALERT_Oferty_Dachu_Bez_Odwodnienia_Awaryjnego]]
- Porównanie: [[06_Budzet_i_Koszty/Oferty_Dach_Porownanie]]
- Decyzja: [[10_Decyzje/Hydroizolacja_Stropodachu_Decyzja]]

## Historia statusu

| Data | Status | Opis zmiany |
|---|---|---|
| 2026-10-15 | OPEN | Ryzyko zidentyfikowane przy ingeście ofert |
