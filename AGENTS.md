# Wyzwanie 100 DNI — instrukcje dla agenta

Pracuj po polsku. Przed planowaniem przeczytaj `RULES.md` i `STATUS.md`, a następnie bieżące dane w prywatnym Google Sheets „100 days challenge”. Arkusz ma pięć zakładek: „Konfiguracja”, „Plan (treningi i kcal)”, „Plan (posiłki)”, „Baza posiłków i produktów” i „Dziennik”. Jeśli znajdziesz kilka plików o tej nazwie, ustal właściwy. Repozytorium zawiera instrukcje, nie arkusz ani dane użytkownika.

## Sposób pracy

- Pomagaj redukować masę z zachowaniem sprawności i świeżości do sędziowania. Oddzielaj dane rzeczywiste, szacunki, plany i braki danych. Nie wymyślaj pomiarów ani wykonanych treningów.
- W poniedziałek zaplanuj okres do środy następnego tygodnia włącznie. Zacznij od historii, regeneracji, dostępności i obsady meczów. Samodzielnie dobierz treningi; nie korzystaj z gotowego schematu biegania. Zasady posiłków i budżetu są w `RULES.md`.
- Zachowaj posiłki NTFY wybrane na bieżący poniedziałek–środę. Dobierz NTFY od czwartku do następnej środy, a treningi i dodatki na następny poniedziałek–środę traktuj jako wstępne do kolejnego przeglądu. Nie zmieniaj wykonanej historii.
- Na polecenie „Szukaj Produktu” lub „Szukaj Przepisu” zastosuj odpowiedni skill z `.agents/skills/`. Pokaż użytkownikowi kandydatów produktu lub jeden konkretny przepis; dodaj do bazy dopiero po jego wyraźnym zatwierdzeniu. Potem możesz użyć zatwierdzonej pozycji w planie. Gdy użytkownik zgłosi dodatkowe jedzenie lub zmianę porcji, popraw plan i podsumowania. Nie sprawdzaj dostępności w konkretnym Lidlu.
- Zegarek jest w reklamacji. Do jego powrotu korzystaj z Dziennika i informacji użytkownika, bez żądania bieżących danych Garmina. Wybrana baza wydatku dnia bez treningu jest w prywatnej Konfiguracji. Wydatek treningu szacuj dopiero po ustaleniu sesji; nie wpisuj szacunków do pól Garmina. Integracja Garmina nie jest wdrożona.

## Arkusz i prywatność

- Użytkownik autoryzował odczyt, edycję i kopie zapasowe tego arkusza przez połączoną wtyczkę Google Drive. Przed edycją zrób kopię na Drive z datą i godziną Europe/Warsaw, odczytaj docelowe komórki, formuły i walidację, a po zapisie sprawdź wynik. Nie usuwaj danych ani poprzednich tygodni. Nie zmieniaj udostępniania plików.
- Zachowaj pięć prostych zakładek i ich istniejące formuły. Trening z godziną, czasem, wariantem i uwagami opisuj w jednej komórce. Posiłki planuj z konkretną gramaturą; checkbox potwierdza zjedzenie całej porcji, a niezaznaczony posiłek oznacza brak potwierdzenia. Dziennik pokazuje wykonanie i pomiary. Szczegóły pól są w `RULES.md`.
- Repozytorium jest publiczne: nie zapisuj tu pomiarów, danych zdrowotnych, planów z danymi osobowymi, eksportów, prywatnego adresu arkusza ani danych logowania. Hasła i tokeny Garmina pozostają poza projektem. Nie twórz lokalnego XLSX, jeśli użytkownik go nie potrzebuje.
- Po zmianach merytorycznych aktualizuj krótko `STATUS.md`. Sprawdzaj sumy i jednostki, ale nie rozbudowuj infrastruktury dla prostych poprawek. Projekt działa na żądanie; nie deklaruj automatyzacji ani połączenia z Garminem przed ich wdrożeniem.
