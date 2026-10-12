# Stan projektu na 12 października 2026

## Cel

100 dni redukcji masy z utrzymaniem zdrowego odżywiania i treningów dostosowanych do pracy sędziego piłkarskiego. Data startu i liczbowy cel nie zostały jeszcze ustalone.

## Gotowe

- Draft `data/Wyzwanie_100_DNI_draft.xlsx` z dwiema zakładkami: „Plan i dziennik” oraz „Posiłki”.
- Plan i pomiary na 100 dni, baza 80 posiłków oraz 600 miejsc na wpisy posiłków. Daty pojawiają się po wpisaniu daty startu w B4 pierwszej zakładki.
- Oddzielne porcje planowane i zjedzone. Automatyczne dzienne sumy planowanych kcal, białka, węglowodanów, tłuszczu i cukrów. W dzienniku są też sumy zapisanych zjedzonych kcal i cukrów; szczegóły pozostałych makroskładników wykonania są w rozpisce posiłków.
- Średnia masy z siedmiu dni, pokazywana od trzech ważnych pomiarów w tym oknie.
- Sprawdzenie obliczeń dla planu i wykonania, zera i braków cukrów, powtórzonych ID posiłku, braku raportu wykonania, średniej masy oraz ostatniego dnia wyzwania. Dane użyte wyłącznie do sprawdzenia usunięto z dostarczonego draftu.
- Ustalenia i instrukcja w `RULES.md`; reguły agentowe w `AGENTS.md`.

## Ustalenia użytkownika

- Zaczynamy prosto. Użytkownik chce kontynuować w Codexie w trybie agentowym.
- Brak integracji Google Drive: użytkownik nie chce przyznawać możliwości usuwania swoich plików. Nie proponuj tej integracji ponownie dla tego projektu.
- Dane Garmina: wybrano `python-garminconnect`. Importer nie został jeszcze napisany ani podłączony do konta.
- NTFY: dwa pudełka dziennie, obiad i kolacja. Opisy są wprowadzane ręcznie; użytkownik prześle przykłady. Cukry są dla niego istotnym parametrem. Powód dodatkowego ograniczania cukru nie jest jeszcze znany.
- Obsada i sugerowane treningi biegowe przychodzą w poniedziałek. Treningi są sugestiami, nie bezwzględnymi poleceniami.
- Piątek/sobota: wybór NTFY na poniedziałek–środę. Poniedziałek: dopasowanie własnych dodatków do już zamówionych dań i wybór pudełek na kolejne dni. Uwzględniamy również niedzielę.
- Termin NTFY: dwa dni przed dostawą do 16:00; licznik konkretnego zamówienia ma pierwszeństwo.
- Pomiary raz tygodniowo są akceptowalne dla użytkownika. Zaproponowano masę trzy razy tygodniowo, talię raz tygodniowo, biodra i udo opcjonalnie co cztery tygodnie. Częstotliwość wymaga jeszcze jego wyboru.
- Użytkownik oczekuje krótkiej, sprawnej pracy. Nie rozbudowuj prostego zadania w wieloetapowy system.

## Najbliższy krok

Zbierz profil użytkownika i przykład opisu dania NTFY. Uzgodnij potrzebne kolumny przed dalszą rozbudową arkusza. Następnie przygotuj odczytowy importer Garmina według `scripts/README.md` i pierwszy realny plan po otrzymaniu danych.

## Niewdrożone

Importer Garmina, scraper NTFY, automatyczne cykliczne uruchamianie, integracja kalendarza. Nie ma logowania do zewnętrznych kont, API kluczy ani realnych pomiarów użytkownika.
