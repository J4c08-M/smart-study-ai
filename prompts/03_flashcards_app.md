# 🎴 Zrób własną aplikację do nauki (jak Anki / Quizlet) w Claude

> Claude potrafi nie tylko wygenerować fiszki jako tekst — może zbudować **interaktywną aplikację do nauki**, która działa w przeglądarce, podobnie do Anki czy Quizleta. Ten przewodnik pokazuje jak to zrobić.

---

## Na czym to polega?

Claude tworzy tzw. **artefakty** — interaktywne aplikacje (HTML/React), które wyświetlają się od razu w oknie rozmowy. Możesz poprosić go o zbudowanie:

- 🎴 **Fiszek** — klikasz, karta się obraca, pokazuje odpowiedź
- 📝 **Quizu** — pytania wielokrotnego wyboru z punktacją
- 🔁 **Powtórek z systemem oceniania** — oznaczasz „umiem / nie umiem", aplikacja pilnuje czego się uczyć (zasada powtórek rozłożonych w czasie, jak w Anki)
- 🃏 **Trybu „dopasuj pary"** — łączenie pojęć z definicjami (jak Quizlet Match)

---

## Krok po kroku

### Krok 1 — Przygotuj materiał
Wgraj plik (slajdy, notatki, PDF) albo wklej tekst, z którego mają powstać fiszki.

### Krok 2 — Poproś o aplikację
Napisz wprost, czego chcesz. Przykłady promptów:

```
Na podstawie wgranych slajdów stwórz interaktywną aplikację do fiszek.
Karta po kliknięciu ma się obracać i pokazywać odpowiedź.
Dodaj przyciski "Umiem" / "Powtórz".
```

```
Zrób mi quiz z 15 pytaniami wielokrotnego wyboru z tego materiału.
Po zakończeniu pokaż wynik i które odpowiedzi były błędne.
```

```
Stwórz aplikację typu Quizlet "dopasuj pary" — pojęcie do definicji,
z tego rozdziału o antybiotykach.
```

### Krok 3 — Ucz się i iteruj
Aplikacja pojawi się obok rozmowy. Możesz prosić o zmiany:
```
Dodaj licznik postępu.
Wymieszaj kolejność kart losowo.
Dodaj tryb tylko z kartami, które oznaczyłem "Powtórz".
```

### Krok 4 — Zapisywanie postępów (opcjonalnie)
Poproś Claude, żeby aplikacja **zapamiętywała Twój postęp** między sesjami:
```
Spraw, żeby aplikacja zapamiętywała które karty już umiem,
nawet po zamknięciu i ponownym otwarciu.
```

---

## Wskazówki

- **Im konkretniejszy prompt, tym lepsza aplikacja** — określ wygląd, funkcje, liczbę kart.
- **Możesz łączyć z komendami** — np. najpierw `/flashcards` (tekst), a potem „zamień te fiszki w interaktywną aplikację".
- **Materiał z Dysku Google** — jeśli masz połączony Dysk, możesz poprosić: „zrób fiszki z prezentacji X z mojego Dysku".
- **Eksport** — możesz poprosić o listę fiszek w formacie gotowym do importu do prawdziwego Anki (CSV: przód; tył).

```
Wyeksportuj te fiszki jako CSV gotowy do importu w Anki (kolumna przód, kolumna tył).
```

---

## Pomysły na zastosowanie

| Materiał | O co poprosić |
|---|---|
| Slajdy z farmakologii | Fiszki lek → mechanizm + działania niepożądane |
| Atlas anatomii | Quiz „wskaż strukturę" z opisami |
| Notatki z interny | Tryb powtórek z oznaczaniem trudnych zagadnień |
| Lista pojęć | Aplikacja „dopasuj pary" pojęcie–definicja |

---

*Część projektu Smart Study AI (CC BY 4.0).*
