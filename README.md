# Wyzwanie 100 DNI

Repozytorium przechowuje instrukcje agenta. Bieżący plan, baza posiłków i Dziennik znajdują się w prywatnym Google Sheets „100 days challenge”. W repozytorium nie ma kopii arkusza ani danych osobowych.

- `AGENTS.md` — zasady działania agenta i pracy z arkuszem.
- `RULES.md` — uzgodniony proces treningów, żywienia i pomiarów oraz źródła.
- `scripts/README.md` — zakres przyszłej, odczytowej integracji Garmina.
- `.agents/skills/szukaj-produktu/` i `.agents/skills/szukaj-przepisu/` — wyszukiwanie i dodawanie pozycji do bazy po zatwierdzeniu przez użytkownika. Wywołania: „Szukaj Produktu” i „Szukaj Przepisu”.
- `.agents/skills/dodaj-produkt/` i `.agents/skills/dodaj-przepis/` — dodawanie na podstawie zdjęcia, opisu lub linku od użytkownika, po sprawdzeniu porcji i makroskładników. Wywołania: „Dodaj Produkt” i „Dodaj Przepis”.

Planowanie odbywa się w poniedziałek do środy kolejnego tygodnia włącznie. Agent odczytuje historię i obsadę, układa treningi, dobiera posiłki NTFY i dodatki z bazy, a następnie zapisuje plan w Google Sheets. Na razie pracuje na żądanie. Integracja Garmina nie jest jeszcze dostępna.

Aby kontynuować w nowej sesji Codexa, otwórz repozytorium i poproś: „Przeczytaj AGENTS.md i RULES.md. Kontynuuj Wyzwanie 100 DNI na podstawie prywatnego arkusza Google Sheets «100 days challenge»”.
