# Stan projektu na 12 października 2026

## Cel

100 dni redukcji masy z utrzymaniem zdrowego odżywiania i treningów dostosowanych do pracy sędziego piłkarskiego. Data startu i liczbowy cel nie zostały jeszcze ustalone.

## Gotowe

- Bieżące źródło planu i pomiarów: prywatny arkusz Google Sheets „100 days challenge”, zakładki „Plan i dziennik” i „Posiłki”. Agent odnajduje go przez Google Drive według instrukcji AGENTS.md; adresu i identyfikatora nie publikujemy.
- Migracja draftu `data/Wyzwanie_100_DNI_draft.xlsx` do powyższego, wcześniej pustego arkusza Google Sheets. Zachowano istniejący link; XLSX pozostaje archiwalną kopią.
- Sprawdzono przez API zgodność wartości, wszystkich 7300 formuł, 1380 reguł walidacji i formatowania komórek z natywnym importem; nie wykryto błędów formuł. Zachowano zamrożone nagłówki, formatowanie warunkowe i wymiary układu; strefa czasu Europe/Warsaw. Podgląd wizualny w przeglądarce nie był dostępny.
- Na Google Drive zachowano kopię „100 days challenge — kopia importu 2026-10-12” przed dalszymi zmianami.
- Plan i pomiary na 100 dni, baza 80 posiłków oraz 600 miejsc na wpisy posiłków. Daty pojawiają się po wpisaniu daty startu w B4 pierwszej zakładki.
- Oddzielne porcje planowane i zjedzone. Automatyczne dzienne sumy planowanych kcal, białka, węglowodanów, tłuszczu i cukrów. W dzienniku są też sumy zapisanych zjedzonych kcal i cukrów; szczegóły pozostałych makroskładników wykonania są w rozpisce posiłków.
- Średnia masy z siedmiu dni, pokazywana od trzech ważnych pomiarów w tym oknie.
- Sprawdzenie obliczeń dla planu i wykonania, zera i braków cukrów, powtórzonych ID posiłku, braku raportu wykonania, średniej masy oraz ostatniego dnia wyzwania. Dane użyte wyłącznie do sprawdzenia usunięto z dostarczonego draftu.
- Ustalenia i instrukcja w `RULES.md`; reguły agentowe w `AGENTS.md`.

## Ustalenia użytkownika

- Zaczynamy prosto. Użytkownik chce kontynuować w Codexie w trybie agentowym.
- 12 października 2026 użytkownik zmienił wcześniejsze ustalenie i zatwierdził przeniesienie danych z GitHuba do Google Sheets oraz aktualizację instrukcji agenta. Korzystamy z połączonej wtyczki Google Drive do odczytu, aktualizacji i kopii wskazanego arkusza. Zakaz usuwania plików i zmiany udostępniania pozostaje w mocy.
- Dane Garmina: wybrano `python-garminconnect`. Importer nie został jeszcze napisany ani podłączony do konta.
- NTFY: dwa pudełka dziennie, obiad i kolacja. Opisy są wprowadzane ręcznie; użytkownik prześle przykłady. Cukry są dla niego istotnym parametrem. Powód dodatkowego ograniczania cukru nie jest jeszcze znany.
- Obsada i sugerowane treningi biegowe przychodzą w poniedziałek. Treningi są sugestiami, nie bezwzględnymi poleceniami.
- Piątek/sobota: wybór NTFY na poniedziałek–środę. Poniedziałek: dopasowanie własnych dodatków do już zamówionych dań i wybór pudełek na kolejne dni. Uwzględniamy również niedzielę.
- Termin NTFY: dwa dni przed dostawą do 16:00; licznik konkretnego zamówienia ma pierwszeństwo.
- Pomiary raz tygodniowo są akceptowalne dla użytkownika. Zaproponowano masę trzy razy tygodniowo, talię raz tygodniowo, biodra i udo opcjonalnie co cztery tygodnie. Częstotliwość wymaga jeszcze jego wyboru.
- Użytkownik oczekuje krótkiej, sprawnej pracy. Nie rozbudowuj prostego zadania w wieloetapowy system.

## Najbliższy krok

Rozpoczęto planowanie tygodnia. Potwierdzone ustalenia i informacje użytkownika zapisano w prywatnym Google Sheets po utworzeniu kopii zapasowej. Plan treningów i jedzenia pozostaje do ustalenia. Najpierw uzupełnij dane potrzebne do doboru obciążeń; następnie profil, zamówione pudełka i opis dania NTFY. Szczegóły osobowe pozostają w prywatnym arkuszu. Odczytowy importer Garmina według `scripts/README.md` jest późniejszym etapem.

## Niewdrożone

Importer Garmina, scraper NTFY, automatyczne cykliczne uruchamianie, integracja kalendarza. Google Sheets jest połączony i dostępny do pracy na żądanie. Nie ma automatycznej synchronizacji z XLSX, logowania do Garmina ani realnych pomiarów użytkownika.
