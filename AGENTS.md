# Wyzwanie 100 DNI — reguły pracy Codexa

## Zacznij tutaj

Pracuj po polsku. Przy pierwszym zadaniu przeczytaj `STATUS.md`, `RULES.md` oraz pliki w `inputs/`, które użytkownik udostępnił. Źródłem planu i pomiarów jest prywatny arkusz Google Sheets „100 days challenge”. Odnajdź go przez wyszukiwanie w połączonej wtyczce Google Drive, odczytaj metadane i potwierdź dwie zakładki: „Plan i dziennik” i „Posiłki”. Pomiń pliki z dopiskiem „kopia importu”. Jeśli jest więcej niż jeden pasujący arkusz, poproś użytkownika o wskazanie właściwego. Prywatnego URL ani identyfikatora nie zapisuj w publicznym repozytorium. Plik `data/Wyzwanie_100_DNI_draft.xlsx` pozostaje archiwalnym draftem, nie bieżącym źródłem danych. `README.md` opisuje uruchomienie projektu.

Pomagaj prowadzić redukcję przez 100 dni z zachowaniem sprawności i świeżości potrzebnej sędziemu piłkarskiemu. Nie zakładaj parametrów ciała, daty startu, docelowych kalorii ani możliwości treningowych, zanim użytkownik ich nie poda. Rozróżniaj ustalone zasady, propozycje, pomiary i brak danych.

## Zakres działań

- Możesz samodzielnie czytać i edytować pliki tego projektu, przygotowywać tygodniowe plany, liczyć dane oraz tworzyć potrzebne skrypty. Przy prostych poprawkach wykonuj najkrótszy potrzebny zakres pracy.
- Użytkownik zatwierdził używanie połączonej wtyczki Google Drive do odczytu i aktualizacji wskazanego arkusza Google Sheets oraz tworzenia jego kopii zapasowych i eksportów. Nie usuwaj plików z Google Drive ani nie zmieniaj ich udostępniania. Nie rozszerzaj działań na inne pliki bez zlecenia.
- Nie usuwaj oryginalnych danych, pomiarów ani poprzednich tygodni. Przed edycją arkusza utwórz na Google Drive kopię zapasową z datą i godziną Europe/Warsaw. Zwykły odczyt nie wymaga kopii. Przed zapisem odczytaj metadane, dokładne zakładki i docelowe zakresy wraz z formułami oraz walidacją; po zapisie odczytaj zmienione komórki i sprawdź obliczenia. Nie nadpisuj nowszych danych arkusza archiwalnym XLSX.
- Repozytorium GitHub przechowuje instrukcje i kod projektu. Nie publikuj w nim danych zdrowotnych, pomiarów ani eksportów zawierających dane osobowe; bieżące dane pozostają w prywatnym arkuszu Google Sheets. Nie zapisuj haseł, tokenów ani kluczy w arkuszu, raportach lub plikach instrukcji. Logowanie do Garmina ma odbywać się lokalnie.
- Integracja Garmin jest zaakceptowanym kierunkiem rozwoju. Najpierw zbuduj importer danych odczytowych przez `python-garminconnect`; nie dodawaj operacji zmieniających lub usuwających dane konta. Awaryjnie obsłuż eksport Garmin Connect.
- NTFY wprowadzamy ręcznie z opisów lub zrzutów ekranu. Scraper pozostaje późniejszym etapem.

## Planowanie

- Obsada meczowa jest punktem odniesienia. Proponowane treningi biegowe są sugestiami: możesz je zmieniać lub pominąć, krótko wyjaśniając istotne zmiany.
- Piątek lub sobota: wybór pudełek na poniedziałek–środę przed terminem NTFY. Poniedziałek wieczorem: ocena wyników, obsada, treningi, dodatki do zamówionych pudełek oraz jedzenie na czwartek–niedzielę.
- Posiłki układaj według ich składu, treningu, godzin i preferencji. Nazwa „obiad” lub „kolacja” nie narzuca godziny.
- Zachowaj dwie zakładki arkusza. Planowane i zjedzone porcje są oddzielnymi polami. Brak wykonania oznacza brak raportu, a zero oznacza pominięcie.
- Uwzględniaj cukry ogółem. Są częścią węglowodanów. Brak cukrów w opisie oznacza brak danych. Nie wyznaczaj ilości cukrów wolnych z samej wartości „w tym cukry”.

## Jakość i ciągłość

Wyliczenia wykonuj kodem lub formułami. Po istotnej zmianie sprawdź sumy, jednostki i przypadki braku danych. Nie rozbudowuj infrastruktury ani zestawu testów dla małych, odwracalnych poprawek. Po zmianie arkusza zachowaj istniejące formuły, strukturę, daty i dane oraz sprawdź zmienione obliczenia.

Korzystaj z wiarygodnych wytycznych dla ważnych zaleceń zdrowotnych. Oceniaj trend masy i talii wraz z formą, regeneracją i wykonaniem jedzenia. Kalorie Garmina traktuj jako szacunek, z rozróżnieniem kalorii aktywnych i całkowitych.

Po zakończeniu zadania krótko zapisz w `STATUS.md`: co wykonano, czego brakuje i jaki jest następny krok. Nie twierdź, że importer, harmonogram lub synchronizacja działają, dopóki nie zostały wdrożone i sprawdzone. Ten projekt na początku działa na żądanie użytkownika.
