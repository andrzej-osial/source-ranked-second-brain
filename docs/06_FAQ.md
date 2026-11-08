# FAQ

### Dlaczego nie opublikować po prostu własnej bazy jako przykładu?

Bo prawdziwa baza budowy to w praktyce zbiór danych osobowych i poufnych:

- **Prywatność i RODO.** Imiona, nazwiska, telefony i e-maile wykonawców, projektantów, inspektorów, sąsiadów. Numer działki i adres jednoznacznie wskazują właściciela w publicznych rejestrach. Publikując je, stajesz się administratorem danych cudzych osób bez podstawy prawnej.
- **Tajemnica ofert.** Oferty, ceny jednostkowe i warunki umów to często tajemnica przedsiębiorstwa oferenta. Publiczne porównanie „firma X jest droższa o 20%" może naruszać jego interesy, a nawet zostać uznane za czyn nieuczciwej konkurencji.
- **Bezpieczeństwo.** Harmonogram (kiedy na budowie są materiały, kiedy nikogo nie ma), rzuty domu, zdjęcia — to gotowa informacja dla złodzieja.
- **Historia git.** Usunięcie pliku w nowym commicie **nie usuwa go z historii**. Wszystko, co raz trafiło do publicznego repo, jest do odzyskania (oraz w forkach i kopiach). Dlatego to repozytorium jest szablonem z fikcyjnym przykładem zbudowanym od zera, a nie oczyszczoną kopią prawdziwej bazy.
- **Twój adres e-mail w commitach.** Przed pierwszym commitem do publicznego repo ustaw adres `noreply` z GitHuba (`git config user.email`).

Dobra praktyka: prywatne repo dla własnej budowy, publiczne — tylko dla metody.

### Czy to działa bez Obsidiana?

Tak. To zwykłe pliki Markdown. Obsidian daje wygodną nawigację po linkach `[[...]]` i graf powiązań, ale agent pracuje na samych plikach.

### Po co rangi, skoro „wiadomo, co jest prawdą"?

Na budowie nie wiadomo. Ten sam parametr pojawia się w projekcie, w ofercie, w mailu i w rozmowie na placu — często w czterech różnych wersjach. Ranga mówi, której wersji wierzyć i dlaczego, a pewność ma sufit: ustalenie ustne nigdy samo nie stanie się FAKTEM.

### Czemu agent nie może po prostu poprawić wiki, gdy dostanie nową rewizję projektu?

Może — o ile nic nie zostało jeszcze wybudowane. Jeśli twierdzenie jest `frozen` (np. strop już zabetonowany), nowa rewizja projektu nie zmienia rzeczywistości. Zamiast cichej aktualizacji powstaje alert, bo rozjazd projekt–stan faktyczny wymaga decyzji człowieka.

### Czy model nie będzie zmyślał?

Będzie próbował. Metoda zakłada to z góry: lista twierdzeń przed zapisem, obowiązkowe źródło przy każdym zdaniu, `UNVERIFIED` zamiast zgadywania, klasa B na gałęzi i LINT, który raportuje FAKT oparty na słabym źródle.

### Ile to kosztuje pracy?

Ingest jednej oferty to kilka minut przeglądu listy twierdzeń. Zysk pojawia się przy porównaniach i sporach: zamiast przekopywać maile, pytasz `/query` i dostajesz odpowiedź z odnośnikami do źródeł.

### Gdzie trzymać pliki PDF i zdjęcia?

W `raw/` lokalnie lub w prywatnym repo. `.gitignore` w tym szablonie domyślnie wyklucza binaria (PDF, zdjęcia, dokumenty biurowe).
