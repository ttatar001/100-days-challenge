# Wyzwanie 100 DNI w Codexie

Instrukcje i kod projektu przechowujemy w repozytorium GitHub. Bieżące plany, posiłki i pomiary prowadzimy w prywatnym arkuszu Google Sheets.

## Arkusz

Prywatny arkusz Google Sheets „100 days challenge”. Agent odnajduje go przez połączoną wtyczkę Google Drive zgodnie z AGENTS.md. Adres i identyfikator pozostają poza publicznym repozytorium.

Dwie zakładki: „Plan i dziennik” i „Posiłki”. Arkusz zawiera draft przeniesiony z `data/Wyzwanie_100_DNI_draft.xlsx`: plan na 100 dni, bazę 80 posiłków i 600 miejsc na wpisy posiłków. Daty pojawiają się po wpisaniu daty startu w B4 zakładki „Plan i dziennik”; data startu i profil nadal wymagają ustalenia.

## Kontynuowanie pracy

1. Otwórz repozytorium w Codexie.
2. Korzystaj z połączonej wtyczki Google Drive do wskazanego arkusza.
3. Poleć agentowi:

> Przeczytaj AGENTS.md, STATUS.md i RULES.md. Kontynuujemy Wyzwanie 100 DNI. Źródłem planu i pomiarów jest arkusz Google Sheets wskazany w AGENTS.md. Przed edycją utwórz kopię na Drive; nie usuwaj plików ani nie zmieniaj udostępniania. Zacznij od zebrania brakującego profilu i analizy opisu NTFY, który prześlę. Zachowaj dwie zakładki oraz oddzielne plan i wykonanie. Pracujemy na żądanie, bez cyklicznej automatyzacji.

Historia rozmowy nie przechodzi automatycznie do nowej sesji. Aktualne ustalenia są zapisane w `STATUS.md` i `RULES.md`.

## Pliki

- `AGENTS.md` — instrukcje dla agenta, link do arkusza i zakres działań.
- `STATUS.md` — wykonane elementy, ustalenia i brakujące dane.
- `RULES.md` — zasady treningów, jedzenia, cukrów i pomiarów.
- `data/Wyzwanie_100_DNI_draft.xlsx` — archiwalny draft; bieżące dane są w Google Sheets.
- `inputs/` — opisy NTFY, obsada, sugestie treningów i profil; danych osobowych nie publikujemy w publicznym repozytorium.
- `scripts/README.md` — zakres planowanego, odczytowego importera Garmina.
- `exports/` i `backups/` — katalogi lokalnych eksportów i kopii; plików z danymi osobowymi nie wysyłamy do repozytorium. Kopie bieżącego arkusza tworzymy na Drive.

## Stan integracji

Google Sheets jest dostępny przez połączoną wtyczkę Google Drive. Migracja XLSX była jednorazowa; nie ma automatycznej synchronizacji z plikiem w repozytorium. Importer Garmina, scraper NTFY i cykliczne uruchamianie nie są wdrożone. Logowanie do Garmina pozostaje lokalne; hasła i tokeny nie trafiają do arkusza ani repozytorium.
