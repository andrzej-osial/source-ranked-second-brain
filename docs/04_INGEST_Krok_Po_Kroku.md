# Jak dodać źródło (INGEST) — krok po kroku

Przykład: przyszła nowa oferta na dach (PDF).

## 1. Człowiek: wrzuć plik do `raw/`

```
raw/oferty/dach/2026-11-02_Firma_X_oferta.pdf
```

Nazwa: data dokumentu + nadawca + typ. Nie zmieniaj treści pliku.

## 2. Uruchom

```
/ingest raw/oferty/dach/2026-11-02_Firma_X_oferta.pdf
```

## 3. Agent: gałąź i rejestr (klasa A)

- tworzy gałąź `agent/2026-11-02-ingest-oferta-dach`,
- dopisuje wiersz do `raw/RAW_INDEX.md`: ID, typ `oferta`, ranga 6, data, **ważne do** (z dokumentu),
- jeśli to nowa wersja wcześniejszej oferty — stary wiersz `ZASTĄPIONY`, cytujące go twierdzenia `stale`.

## 4. Agent: streszczenie 1:1 (klasa A)

`15_Knowledge_Base/2026-11-02_Firma_X_oferta.md` — wierne streszczenie + **uwagi redakcyjne** (błędy sum, inna powierzchnia niż w projekcie, brakujące pozycje).

## 5. Agent: lista twierdzeń — STOP

Agent pokazuje listę **przed zapisem**:

```
T-0060 FAKT  r6  Firma X zaoferowała ... za ... zł netto, ważne do ...   → 06_Budzet/Oferty_Dach_Porownanie
T-0061 FAKT  r6  Oferta nie obejmuje obróbek attyk                       → jw.
T-0062 REKOM r8  Powierzchnia w ofercie o 6% większa od projektu         → jw. (Wyprowadzone z: T-0003, T-0060)
Konflikty: brak. Klasa B: zmiana w 06_Budzet (zawsze B).
```

Ty: akceptujesz, poprawiasz albo odrzucasz pozycje. To najważniejszy moment całej metody — tu łapiesz pomyłki modelu, zanim staną się „wiedzą".

## 6. Agent: konflikty i zapis

- szuka sprzeczności w `03_`, `04_`, `05_`, `06_`, `09_`, `10_`,
- stosuje reguły: wyższa ranga → nowsza data → `disputed`,
- klasa A zapisuje od razu, klasa B tylko na gałęzi.

## 7. Agent: porządki i diff

- aktualizuje `CHANGELOG.md`, `00_Dashboard/hot.md`, indeksy,
- tworzy `_ops/diff-2026-11-02-ingest-oferta-dach.md` z sekcją **DECYZJA CZŁOWIEKA WYMAGANA**,
- wypisuje komendę merge i **zatrzymuje się**.

## 8. Człowiek: `/diff-review`

Przechodzisz pozycje klasy B: AKCEPTUJ / ODRZUĆ / ZMIEŃ. Dopiero potem merge do `main`.

Wzór gotowego diffa: [[_ops/diff-2026-10-15-ingest-oferty-dach]].
