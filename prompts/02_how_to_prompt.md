# 🧠 Jak dobrze promptować Claude

> Krótki przewodnik dla studentów: jak formułować polecenia, żeby Claude odpowiadał trafniej, dokładniej i bardziej pod Twoje potrzeby.

---

## Dlaczego to ważne?

Jakość odpowiedzi Claude'a zależy w ogromnym stopniu od tego, **jak** zadasz pytanie. Te same materiały mogą dać powierzchowną notatkę albo dogłębne, egzaminacyjne opracowanie — różnica leży w prompcie.

---

## 7 zasad dobrego promptu

### 1. Bądź konkretny
Zamiast ogólników podaj dokładnie czego chcesz.

| ❌ Słabo | ✅ Dobrze |
|---|---|
| „Opowiedz o cukrzycy" | „Wyjaśnij patofizjologię cukrzycy typu 2 na poziomie 4. roku, z naciskiem na insulinooporność" |

### 2. Podaj kontekst i poziom
Powiedz kim jesteś i do czego potrzebujesz odpowiedzi.
```
Jestem na 3. roku, przygotowuję się do egzaminu z fizjologii.
Wyjaśnij mechanizm potencjału czynnościowego tak, żebym zrozumiał, nie tylko zapamiętał.
```

### 3. Określ format odpowiedzi
Claude dostosuje się, jeśli powiesz jak ma wyglądać wynik.
```
Przedstaw to jako tabelę porównawczą.
Daj mi listę punktową, maksymalnie 7 punktów.
Wyjaśnij w formie krok-po-kroku.
```

### 4. Pracuj iteracyjnie
Nie musisz dostać idealnej odpowiedzi za pierwszym razem. Doprecyzowuj:
```
Za długie — skróć do najważniejszych 5 punktów.
Dodaj przykład kliniczny.
Teraz zrób z tego fiszki.
```

### 5. Podawaj materiał źródłowy
Najlepsze odpowiedzi powstają, gdy Claude pracuje na Twoich plikach. Wgraj slajdy/PDF i odwołuj się do nich:
```
Na podstawie wgranych slajdów wyjaśnij...
Streść TYLKO to, co jest w tym dokumencie.
```

### 6. Proś o rozumowanie, nie tylko o wynik
Dla nauki cenniejsze jest „dlaczego" niż „co".
```
Wyjaśnij krok po kroku, dlaczego tak się dzieje.
Pokaż tok rozumowania klinicznego, nie tylko diagnozę.
```

### 7. Używaj komend skrótu
Jeśli wkleiłeś prompt z tego projektu, korzystaj z gotowych komend (`/summary`, `/quiz`, `/flashcards`...) — oszczędzasz czas i masz spójny format.

---

## Schemat dobrego promptu

```
[KONTEKST] Jestem na 4. roku, uczę się do egzaminu z interny.
[ZADANIE]  Wyjaśnij mi diagnostykę różnicową bólu w klatce piersiowej.
[FORMAT]   Przedstaw jako tabelę: przyczyna | kluczowe objawy | badanie potwierdzające.
[ŹRÓDŁO]   Bazuj na wgranym pliku z wytycznymi.
```

---

## Częste błędy

| Błąd | Skutek | Jak naprawić |
|---|---|---|
| Zbyt ogólne pytanie | Powierzchowna odpowiedź | Dodaj poziom, zakres, format |
| Brak materiału źródłowego | Claude opiera się na wiedzy ogólnej | Wgraj plik / połącz Dysk |
| Wszystko w jednym prompcie | Chaos, pominięte wątki | Rozbij na kroki, pracuj iteracyjnie |
| Brak określenia formatu | Ściana tekstu | Poproś o tabelę / listę / fiszki |

---

## Dla dociekliwych

Anthropic udostępnia oficjalny przewodnik po inżynierii promptów:
[docs.claude.com — Prompt Engineering](https://docs.claude.com/en/docs/build-with-claude/prompt-engineering/overview)

---

*Część projektu Smart Study AI (CC BY 4.0).*
