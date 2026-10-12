# Wyzwanie 100 DNI w Codexie

Pakiet zawiera arkusz i kontekst przeniesiony z rozmowy. To lokalny projekt do kontynuowania pracy z agentem. Historia tej rozmowy nie zostaje automatycznie przeniesiona do nowej sesji; jej ustalenia zapisano w `STATUS.md` i `RULES.md`.

## Uruchomienie

1. Rozpakuj archiwum i zachowaj cały folder `wyzwanie100`.
2. Otwórz ten folder jako projekt w Codexie lub jako folder roboczy w rozszerzeniu IDE. W aplikacji z projektami lokalnymi wybierz go jako folder główny.
3. Użyj trybu z potwierdzaniem działań poza przestrzenią projektu. Nie podłączaj Google Drive.
4. Wyślij agentowi poniższe polecenie.

> Przeczytaj AGENTS.md, STATUS.md i RULES.md. Kontynuujemy Wyzwanie 100 DNI. Zacznij od zebrania brakującego profilu i analizy opisu NTFY, który prześlę. Zachowaj prostą strukturę arkusza. Nie podłączaj Google Drive. Następnie przygotuj lokalny odczytowy importer Garmina przez python-garminconnect. Na razie pracujemy na żądanie, bez cyklicznej automatyzacji.

Jeśli korzystasz z już zainstalowanego Codex CLI, w terminalu otwartym w folderze `wyzwanie100` uruchom `codex`. Codex odczytuje instrukcje `AGENTS.md` z katalogu projektu. Nie jest potrzebne zewnętrzne repozytorium Git do pierwszego etapu pracy.

## Pliki

- `AGENTS.md` — instrukcje dla agenta i zakres działań.
- `STATUS.md` — ustalenia, wykonane elementy i brakujące dane.
- `RULES.md` — zasady treningów, jedzenia, cukrów i pomiarów.
- `data/Wyzwanie_100_DNI_draft.xlsx` — istniejący draft, bez zmiany jego zawartości.
- `inputs/` — opisy NTFY, obsada, sugestie treningów i profil.
- `scripts/README.md` — punkt startowy do budowy importera Garmina.
- `exports/` — miejsce na przyszłe plany i podsumowania.
- `backups/` — miejsce na kopie przed zmianą arkusza.

## Zakres gotowego pakietu

Agent może pracować na plikach po otwarciu folderu w Codexie. Ten pakiet nie uruchamia procesu w tle, nie loguje do Garmina i nie konfiguruje cyklicznych zadań. Są to kolejne kroki implementacji.

Dokumentacja: https://learn.chatgpt.com/docs/projects oraz https://learn.chatgpt.com/docs/agent-configuration/agents-md
