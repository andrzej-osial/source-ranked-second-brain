# Szybki start

## 1. Wymagania

- [Obsidian](https://obsidian.md) (darmowy) — do czytania i nawigacji po linkach `[[...]]`.
- [Claude Code](https://docs.claude.com/en/docs/claude-code) — agent, który czyta `CLAUDE.md` i pracuje na plikach.
- Git — każda zmiana agenta jest widoczna jako diff i odwracalna.

## 2. Pierwsze uruchomienie (demo)

```bash
git clone https://github.com/andrzej-osial/source-ranked-second-brain.git moja-budowa
cd moja-budowa
claude
```

W Obsidianie: *Open folder as vault* → wskaż katalog `moja-budowa`. Zacznij od `00_Dashboard/START.md`.

Wypróbuj w Claude Code:

```
/query Która oferta na dach jest najkorzystniejsza?
/lint
/diff-review
```

## 3. Przejście na własną budowę

1. Usuń dane demo: pliki oznaczone „FIKCYJNE DEMO" w `raw/`, ich streszczenia w `15_Knowledge_Base/` oraz pliki z twierdzeniami T-…  (lista w `CHANGELOG.md`). Zostaw szablony `_TEMPLATE_*` i pliki `README.md`.
2. Wyzeruj `raw/RAW_INDEX.md` (zostaw nagłówek tabeli), `CHANGELOG.md`, `00_Dashboard/hot.md`.
3. Uzupełnij sekcję **Kontekst inwestycji** w `CLAUDE.md`.
4. **Zanim dodasz prawdziwe dokumenty** — przestaw repo na prywatne albo odkomentuj blokadę `raw/` w `.gitignore`. Patrz [[docs/06_FAQ]].
5. Wrzuć pierwszy dokument do `raw/` i uruchom `/ingest raw/projekt/<plik>`.

## 4. Dzienna praca

| Sytuacja | Komenda |
|---|---|
| Nowa oferta, mail, protokół | `/ingest <ścieżka>` |
| Nowa rewizja projektu | `/rewizja <ścieżka>` |
| Pytanie o stan budowy | `/query <pytanie>` |
| Etap zakończony (np. betonowanie) | `/freeze <punkt bez odwrotu>` |
| Przegląd zmian agenta przed merge | `/diff-review` |
| Raz w tygodniu / przed ważną decyzją | `/lint` |
| Koniec sesji / wznowienie | `/handoff`, `/pickup` |
