# 📖 Universal Template — przewodnik po prompcie

> Ten plik **wyjaśnia krok po kroku** co znajduje się w prompcie i jak go poprawnie wypełnić.
> Sam gotowy prompt do skopiowania znajduje się w osobnym pliku: [`00_prompt_only.md`](./00_prompt_only.md).

---

## ⚠️ Disclaimer

> Szablon jest stworzony **wyłącznie w celach edukacyjnych** — aby pomóc studentom w nauce obsługi narzędzi AI i efektywnym uczeniu się na podstawie **własnych, legalnie posiadanych materiałów**.
>
> **Zabrania się** używania go do: reprodukowania materiałów chronionych prawem autorskim, pisania prac za studenta, wprowadzania w błąd egzaminatorów oraz jakiejkolwiek formy nieuczciwości akademickiej.
>
> Claude jest narzędziem wspierającym **rozumienie i naukę** — nie zastępuje pracy własnej studenta.

---

## Jak zacząć

1. Otwórz plik [`00_prompt_only.md`](./00_prompt_only.md)
2. Skopiuj cały blok promptu
3. W Claude: **Settings → „Add instructions to tailor Claude's responses"** → wklej
4. Uzupełnij pola `[FILL IN]` (instrukcje poniżej)

---

## 📌 Sekcja 1: `MY PROFILE` — Twój profil

Tu definiujesz kim jesteś, żeby Claude dostosował poziom i język odpowiedzi.

| Pole | Przykład wypełnienia | Dlaczego to ważne |
|---|---|---|
| Year of study | `4th year, clinical rotations` | Claude dostosuje poziom szczegółowości |
| University / country | `Medical University of Białystok, Poland` | Kontekst lokalnych egzaminów |
| Language | `Polish` lub `Polish for explanations, English for terminology` | Odpowiedzi w preferowanym języku |
| Exam system | `Polish LEK exam` lub `USMLE Step 1` | Claude dobiera styl pytań egzaminacyjnych |

---

## 📌 Sekcja 2: `MY MATERIALS` — Twoje materiały

Ta sekcja mówi Claude'owi, żeby zawsze bazował na Twoich materiałach, a nie na ogólnej wiedzy. Masz kilka sposobów dostarczenia mu materiałów:

### A) Wgrywanie plików w rozmowie
Najprostsza metoda — przeciągnij plik (PDF, slajdy, zdjęcie notatek) bezpośrednio do okna czatu. Claude przeczyta go i będzie na nim pracował.

### B) Dołączenie plików do repozytorium / projektu
Jeśli pracujesz w **Projekcie Claude** (Projects), możesz dodać swoje materiały na stałe do wiedzy projektu — wtedy Claude ma do nich dostęp w każdej rozmowie bez ponownego wgrywania. Możesz tam dołączyć np.:
- skany podręczników i atlasów (legalnie posiadanych)
- własne notatki w PDF
- prezentacje i slajdy udostępnione do nauki
- gotowe zestawy przypadków klinicznych

> ⚠️ Dodawaj wyłącznie materiały, które masz prawo wykorzystywać. Nie udostępniaj publicznie cudzych treści chronionych prawem autorskim.

### C) Połączenie z Dyskiem Google
Claude można skonfigurować tak, aby **przeszukiwał Twój Dysk Google** i pracował na połączonych z nim plikach. Dzięki temu nie musisz wgrywać materiałów ręcznie — Claude sięgnie po nie sam, gdy będą potrzebne.

Jak włączyć:
1. W Claude wejdź w ustawienia konektorów / integracji (sekcja **Connectors** lub **Tools**)
2. Połącz **Google Drive** i autoryzuj dostęp
3. Od teraz możesz prosić np. *„przeszukaj mój Dysk i znajdź notatki o niewydolności serca"* albo *„zrób /summary z prezentacji X z mojego Dysku"*

> Dostępność tej opcji zależy od Twojego planu Claude. Szczegóły: [support.claude.com](https://support.claude.com).

---

## 📌 Sekcja 3: `LEARNING FOCUS` — na czym się skupiasz

Uzupełnij na bieżąco — możesz to zmieniać w trakcie semestru:

```
My current subject / block / rotation: Cardiology, 4th year
Topics I find most difficult: ECG interpretation, heart failure classification
Topics I am confident in: basic cardiac anatomy
```

---

## 📌 Sekcja 4 & 5: `HOW I WANT YOU TO TEACH` + `EXAM PREPARATION MODE`

Określają **jak** Claude ma uczyć: zawsze tłumacząc mechanizmy, prowadząc rozumowanie kliniczne i kończąc krótkim podsumowaniem. Tryb egzaminacyjny dodaje pułapki i mini-testy.

Możesz dodać własne preferencje, np.:
```
I prefer explanations with real-world clinical analogies.
I learn better with tables than with long paragraphs.
```

---

## 📌 Sekcja 6: `QUICK COMMANDS` — komendy skrótu

To jedna z najpotężniejszych funkcji. Zamiast pisać długie polecenia, użyj skrótu:

| Komenda | Co zrobi Claude |
|---|---|
| `/flashcards` | Fiszki z wgranego pliku (PRZÓD / TYŁ) |
| `/quiz` | 5 pytań egzaminacyjnych MCQ z omówieniem |
| `/summary` | Strukturyzowane streszczenie dokumentu |
| `/compare cukrzyca t1 vs t2` | Tabela porównawcza dwóch tematów |
| `/case kardiologia` | Losowy przypadek kliniczny do rozwiązania |
| `/explain` | Wyjaśnienie od podstaw, prostym językiem |
| `/highyield` | Lista najważniejszych faktów do egzaminu |

---

## 📌 Sekcja 7: `FORMAT PREFERENCES` + `SAFETY & SCOPE`

Ostatnie dwie sekcje pilnują, żeby odpowiedzi były czytelne (tabele, nagłówki) oraz bezpieczne — Claude nie wymyśla dawek leków i odsyła do wiarygodnych źródeł (UpToDate, PubMed, Harrison's, Robbins).

---

## 💡 Przykłady promptów po wklejeniu instrukcji

```
Wgrywam slajdy z wykładu. Zrób mi /summary a potem /flashcards.
```
```
/compare AF vs flutter przedsionków
```
```
/case nefrologia — przeprowadź mnie przez przypadek ostrego uszkodzenia nerek.
```
```
/highyield — leki pierwszego rzutu w nadciśnieniu tętniczym, format do LEK.
```

---

## 🔗 Dalej

- 🧠 Chcesz lepiej promptować? Zobacz [`02_how_to_prompt.md`](./02_how_to_prompt.md)
- 🎴 Chcesz zrobić własną aplikację do fiszek (jak Anki/Quizlet)? Zobacz [`03_flashcards_app.md`](./03_flashcards_app.md)

---

*Szablon możesz kopiować, modyfikować i udostępniać zgodnie z licencją projektu (CC BY 4.0).*
