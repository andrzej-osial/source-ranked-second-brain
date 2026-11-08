---
title: "Stropodach — parametry projektowe"
typ: dokument
status: IN_PROGRESS
priorytet: HIGH
tagi: [#architecture, #construction]
updated: 2026-10-15
---

# Stropodach — parametry projektowe

## Twierdzenia

- [T-0001] {status: superseded → T-0004} {pewność: HIPOTEZA} {as-of: 2026-07-02} {ważne-do: none} {wymaga: potwierdzenie-projektanta}
  Ocieplenie stropodachu ma grubość 20 cm (wg wypowiedzi kierownika budowy).
  Źródło: [[raw/korespondencja/2026-07-02_notatka_spotkanie_budowa.md]] (S-007) | ranga: 7
  ⚠️ 2026-10-15: `superseded → T-0004` — projekt techniczny (ranga 3) wygrywa z notatką ze spotkania (ranga 7).

- [T-0002] {status: active} {pewność: FAKT} {as-of: 2026-03-02} {ważne-do: none} {wymaga: —}
  Dach budynku jest płaskim stropodachem niewentylowanym ze spadkiem min. 2% w kierunku wpustów.
  Źródło: [[raw/projekt/PAB_Dom_Przykladowy.md]] (S-001) rozdz. 4.1 | ranga: 4 | rewizja: rev.0

- [T-0003] {status: active} {pewność: FAKT} {as-of: 2026-08-20} {ważne-do: PT-rev-next} {wymaga: —}
  Powierzchnia hydroizolacji stropodachu wraz z wywinięciami na attyki wynosi 172 m².
  Źródło: [[raw/projekt/PT_Stropodach_rev1.md]] (S-002) rys. K-07 | ranga: 3 | rewizja: PT rev.1

- [T-0004] {status: active} {pewność: FAKT} {as-of: 2026-08-20} {ważne-do: PT-rev-next} {wymaga: —}
  Ocieplenie stropodachu to EPS dachowy o średniej grubości 25 cm z warstwą spadkową 2%.
  Źródło: [[raw/projekt/PT_Stropodach_rev1.md]] (S-002) rys. K-07 | ranga: 3 | rewizja: PT rev.1

- [T-0005] {status: active} {pewność: FAKT} {as-of: 2026-08-20} {ważne-do: PT-rev-next} {wymaga: —}
  Odwodnienie stropodachu obejmuje 4 wpusty dachowe i 2 przelewy awaryjne w attyce.
  Źródło: [[raw/projekt/PT_Stropodach_rev1.md]] (S-002) rys. K-07 | ranga: 3 | rewizja: PT rev.1

- [T-0006] {status: disputed} {pewność: HIPOTEZA} {as-of: 2026-09-20} {ważne-do: none} {wymaga: potwierdzenie-projektanta}
  Wywinięcie hydroizolacji na attyce musi mieć min. 15 cm ponad warstwę wierzchnią (stanowisko kierownika budowy).
  Źródło: [[raw/korespondencja/2026-09-20_notatka_spotkanie_dach.md]] (S-006) | ranga: 7
  > ⚠️ Sprzeczność z T-0007 — równa ranga, ta sama data. Rozstrzyga: projektantka. Termin: 2026-10-30. Wpis: [[_ops/diff-2026-10-15-ingest-oferty-dach]].

- [T-0007] {status: disputed} {pewność: HIPOTEZA} {as-of: 2026-09-20} {ważne-do: none} {wymaga: potwierdzenie-projektanta}
  Wywinięcie hydroizolacji na attyce o wysokości 10 cm jest wystarczające (stanowisko przedstawiciela Dachy Alfa).
  Źródło: [[raw/korespondencja/2026-09-20_notatka_spotkanie_dach.md]] (S-006) | ranga: 7
  > ⚠️ Sprzeczność z T-0006 — patrz wyżej.

- [T-0008] {status: stale} {pewność: FAKT} {as-of: 2026-06-10} {ważne-do: PT-rev-next} {wymaga: —}
  Powierzchnia hydroizolacji stropodachu wynosi 165 m².
  Źródło: [[raw/projekt/PT_Stropodach_rev0.md]] (S-009) | ranga: 3 | rewizja: PT rev.0
  # do weryfikacji wobec PT rev.1 (S-002) — źródło ma status ZASTĄPIONY od 2026-08-21.

- [T-0009] {status: active} {pewność: UNVERIFIED} {as-of: 2026-09-20} {ważne-do: none} {wymaga: potwierdzenie-projektanta}
  Attyka od strony ogrodu ma wysokość ok. 40 cm ponad warstwę wierzchnią.
  Źródło: [[raw/korespondencja/2026-09-20_notatka_spotkanie_dach.md]] (S-006) | ranga: 7
  Do weryfikacji: wysokość attyki po zmianie w PT rev.1 — zapytać projektantkę (rysunek przekroju attyki), ewentualnie pomiar na budowie.

## Kontekst

Plik zbiera parametry projektowe stropodachu, z których korzystają: porównanie ofert [[06_Budzet_i_Koszty/Oferty_Dach_Porownanie]], decyzja [[10_Decyzje/Hydroizolacja_Stropodachu_Decyzja]] i ryzyko [[09_Ryzyka_i_Problemy/Ryzyka_Miedzybranzowe/Odwodnienie_Awaryjne_Stropodachu]].

Pokazuje trzy mechanizmy metody naraz: rozstrzygnięcie przez rangę (T-0001 przegrywa z T-0004), spór przy równej randze (T-0006 vs T-0007 — agent nie rozstrzyga) oraz wygaszenie twierdzenia po wejściu nowej rewizji projektu (T-0008).
