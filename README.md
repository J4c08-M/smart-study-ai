<div align="center">

# 🩺 Smart Study AI
## Claude Prompt Template for Medical Students

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightblue.svg)](https://creativecommons.org/licenses/by/4.0/)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.20692545.svg)](https://doi.org/10.5281/zenodo.20692545)
[![Status](https://img.shields.io/badge/status-active-brightgreen)](https://github.com)
[![Made with Claude](https://img.shields.io/badge/made%20with-Claude%20AI-orange)](https://claude.ai)
[![For](https://img.shields.io/badge/for-medical%20students-purple)](https://github.com)

**Polski** | [English summary below](#english-summary)

</div>

---

## 🎯 O projekcie

**Smart Study AI** to gotowy, otwarty szablon instrukcji dla Claude'a (Anthropic), zaprojektowany dla **studentów kierunku lekarskiego**.

Powstał jako inicjatywa edukacyjna — nauka korzystania z narzędzi AI w kontekście akademickim, ze szczególnym uwzględnieniem etycznego i odpowiedzialnego wykorzystania modeli językowych przez studentów medycyny.

> 💡 **Idea przewodnia:** AI nie zastępuje nauki — pomaga uczyć się mądrzej. Szablon jest zaprojektowany tak, aby Claude wspierał *rozumienie*, a nie zapamiętywanie gotowych odpowiedzi.

---

## 👥 Dla kogo?

- studentów kierunku lekarskiego na każdym roku (przedkliniczne i kliniczne)
- osób przygotowujących się do egzaminów (LEK/LDEK, USMLE, OSCE, egzaminy uczelniane)
- każdego, kto chce nauczyć się efektywnie korzystać z AI w nauce medycyny

---

## ⚠️ Disclaimer

> Ten projekt jest stworzony **wyłącznie w celach edukacyjnych**.
>
> Ma pomóc studentom w nauce obsługi narzędzi AI oraz w efektywnym uczeniu się na podstawie **własnych, legalnie posiadanych materiałów**.
>
> **Projekt nie promuje i nie wspiera:** plagiatu, reprodukowania treści chronionych prawem autorskim, używania AI zamiast własnej pracy ani jakiejkolwiek formy nieuczciwości akademickiej.
>
> Claude jest narzędziem **wspierającym rozumienie** — nie zastępuje pracy studenta.

> 📌 Pełne oświadczenie autora na temat rzetelności akademickiej znajdziesz w pliku [**DISCLAIMER.md**](./DISCLAIMER.md).

---

## 📁 Zawartość repozytorium

```
📦 smart-study-ai/
│
├── README.md                          ← Ten plik (strona główna projektu)
├── DISCLAIMER.md                      ← Oświadczenie autora
├── LICENSE                            ← Licencja CC BY 4.0
├── CITATION.cff                       ← Plik cytowania (dla Zenodo / DOI)
│
└── prompts/
    ├── 00_prompt_only.md              ← ⭐ Sam prompt — do skopiowania i uzupełnienia
    ├── 01_universal_template.md       ← Przewodnik wyjaśniający każdą sekcję promptu
    ├── 02_how_to_prompt.md            ← Jak dobrze promptować Claude
    └── 03_flashcards_app.md           ← Jak zrobić aplikację do nauki (Anki / Quizlet)
```

---

## 🚀 Jak używać — Quick Start

### Krok 1 — Skopiuj prompt
Otwórz [`prompts/00_prompt_only.md`](./prompts/00_prompt_only.md) i skopiuj cały blok instrukcji.

### Krok 2 — Wklej w Claude
1. Zaloguj się na [claude.ai](https://claude.ai)
2. Kliknij swój avatar → **Settings**
3. Znajdź sekcję **„Add instructions to tailor Claude's responses"**
4. Wklej skopiowany blok i zapisz ✅

### Krok 3 — Uzupełnij pola `[FILL IN]`
Zamień pola `[FILL IN: ...]` na swoje dane (rok studiów, język, przedmiot, egzamin).
Nie wiesz co oznacza dana sekcja? Wszystko wyjaśnia [`01_universal_template.md`](./prompts/01_universal_template.md).

### Krok 4 — Używaj komend skrótu

| Komenda | Efekt |
|---|---|
| `/flashcards` | Fiszki z wgranego pliku |
| `/quiz` | 5 pytań MCQ z omówieniem |
| `/summary` | Strukturyzowane streszczenie dokumentu |
| `/compare A vs B` | Tabela porównawcza dwóch tematów |
| `/case [temat]` | Interaktywny przypadek kliniczny |
| `/explain` | Wyjaśnienie od podstaw |
| `/highyield` | Lista faktów do egzaminu |

---

## 📚 Praca z własnymi materiałami

Claude działa najlepiej, gdy uczy się z **Twoich** materiałów. Masz trzy sposoby:

### 1. Wgrywanie plików w rozmowie
Przeciągnij plik (PDF, slajdy, zdjęcie notatek) do okna czatu — Claude przeczyta go i będzie na nim pracował.

### 2. Dołączanie plików do Projektu Claude
W **Projektach Claude** możesz dodać materiały na stałe do wiedzy projektu — wtedy Claude ma do nich dostęp w każdej rozmowie bez ponownego wgrywania. Możesz dołączyć np. skany legalnie posiadanych podręczników, własne notatki PDF, prezentacje czy gotowe zestawy przypadków klinicznych.

> ⚠️ Dodawaj wyłącznie materiały, które masz prawo wykorzystywać. Nie udostępniaj publicznie cudzych treści chronionych prawem autorskim.

### 3. Połączenie z Dyskiem Google
Claude można skonfigurować tak, aby **przeszukiwał Twój Dysk Google** i pracował na zapisanych tam plikach — bez ręcznego wgrywania. Włączysz to w ustawieniach konektorów (sekcja **Connectors / Tools**), łącząc Google Drive. Potem wystarczy poprosić, np. *„przeszukaj mój Dysk i zrób /summary z prezentacji o niewydolności serca"*.

> Dostępność tej opcji zależy od planu Claude. Szczegóły: [support.claude.com](https://support.claude.com).

---

## 🎴 Zrób własną aplikację do nauki

Claude potrafi zbudować **interaktywną aplikację do nauki** działającą w przeglądarce — podobną do Anki lub Quizleta. W każdej chwili możesz poprosić go o:

- fiszki, które obracają się po kliknięciu
- quiz z punktacją i podsumowaniem błędów
- tryb powtórek z oznaczaniem „umiem / powtórz" (jak w Anki)
- tryb „dopasuj pary" pojęcie–definicja (jak w Quizlet)

Przykład:
```
Na podstawie wgranych slajdów stwórz interaktywną aplikację do fiszek.
Karta po kliknięciu obraca się i pokazuje odpowiedź. Dodaj przyciski "Umiem" / "Powtórz".
```

Pełny przewodnik (z eksportem do prawdziwego Anki): [`prompts/03_flashcards_app.md`](./prompts/03_flashcards_app.md).

---

## 🧠 Jak dobrze promptować?

Jakość odpowiedzi Claude'a zależy od tego, jak zadasz pytanie. Krótki przewodnik z 7 zasadami dobrego promptu, schematem i częstymi błędami znajdziesz w [`prompts/02_how_to_prompt.md`](./prompts/02_how_to_prompt.md).

---

## 💬 Przykłady użycia

```
Wgrywam slajdy z wykładu o niewydolności serca.
Zrób mi /summary a potem /flashcards.
```
```
/compare AF vs flutter przedsionków
```
```
/case nefrologia — ostre uszkodzenie nerek, 3. rok studiów
```
```
/highyield — leki pierwszego rzutu w nadciśnieniu, format do egzaminu LEK
```

---

## 📜 Licencja

Ten projekt jest udostępniony na licencji **Creative Commons Attribution 4.0 International (CC BY 4.0)**.

[![CC BY 4.0](https://licensebuttons.net/l/by/4.0/88x31.png)](https://creativecommons.org/licenses/by/4.0/)

Możesz kopiować, modyfikować i udostępniać — także komercyjnie — pod warunkiem podania autora i wskazania zmian.

> **Dlaczego CC BY 4.0, a nie MIT?** Ten projekt to dokumentacja i szablon tekstowy, nie kod programistyczny. CC BY 4.0 jest standardem w środowisku naukowym, rozpoznawanym przez Zenodo i DOI, i pasuje do projektu edukacyjnego przeznaczonego do cytowania i udostępniania.

---

## 🔬 DOI i Zenodo

To repozytorium może zostać połączone z platformą **[Zenodo](https://zenodo.org)** w celu nadania mu stałego identyfikatora naukowego **DOI**, który umożliwia trwałe cytowanie w pracach akademickich.

**DOI tego repozytorium:**
`https://doi.org/10.5281/zenodo.20692545`

> 📘 Nie wiesz jak nadać DOI? Cały proces krok po kroku opisałem w powiązanym projekcie [**open-science-starter**](https://github.com/J4c08-M/open-science-starter).

---

## 🔗 Projekty powiązane

| Projekt | Opis |
|---|---|
| **smart-study-ai** *(to repozytorium)* | Szablon promptów Claude dla studentów medycyny |
| [**open-science-starter**](https://github.com/J4c08-M/open-science-starter) | Przewodnik: jak opublikować projekt na GitHub, nadać DOI przez Zenodo i połączyć ORCID |

---

## 👤 Autor

Projekt stworzony jako inicjatywa edukacyjna przez studenta medycyny uczącego się korzystania z narzędzi AI i open-source.

---

<a name="english-summary"></a>

## 🇬🇧 English Summary

**Smart Study AI** is a universal, configurable **Claude AI prompt template** for medical students. It includes:

- a clean, ready-to-paste prompt with fill-in-the-blank fields ([`00_prompt_only.md`](./prompts/00_prompt_only.md))
- a section-by-section explanatory guide ([`01_universal_template.md`](./prompts/01_universal_template.md))
- a guide on effective prompting ([`02_how_to_prompt.md`](./prompts/02_how_to_prompt.md))
- a guide to building interactive Anki/Quizlet-style study apps in Claude ([`03_flashcards_app.md`](./prompts/03_flashcards_app.md))
- shortcut commands (`/flashcards`, `/quiz`, `/summary`, `/compare`, `/case`, `/explain`, `/highyield`)
- guidance on using your own materials, Google Drive integration, and an ethical disclaimer

The template is subject-agnostic and works for any medical course. It is part of a series of educational repositories, alongside [**open-science-starter**](https://github.com/J4c08-M/open-science-starter) — a guide to publishing on GitHub, obtaining a DOI via Zenodo, and linking ORCID.

**License:** CC BY 4.0 | **Status:** Educational / Open Source

---

<div align="center">

*Jeśli projekt był pomocny — zostaw ⭐ na GitHubie!*
*If this was useful — leave a ⭐ on GitHub!*

</div>
