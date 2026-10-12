# Importer Garmina — następne zadanie Codexa

Nie ma jeszcze implementacji ani aktywnego połączenia. Przygotuj prosty skrypt Python korzystający z aktualnej wersji `python-garminconnect`: https://github.com/cyberjunky/python-garminconnect

Najpierw sprawdź dokumentację aktualnej wersji, sygnatury metod i obsługę logowania. Nie opieraj kodu na nieaktualnym przykładzie uwierzytelniania. Na start uruchamianie ręczne na lokalnym komputerze jest wystarczające.

Zakres pierwszej wersji:

1. Odczyt ostatnich 14 dni: aktywności, czas, dystans, tętno, kalorie oraz sen i dostępne podsumowania dobowe.
2. Wyraźne rozróżnienie kalorii aktywnych i całkowitych. Zapisywanie jednostek, dat i źródła.
3. Brak danych jako brak, z zachowaniem rzeczywistych zer. Nie zakładaj, że każdy model zegarka udostępnia wszystkie metryki.
4. Zapis danych źródłowych w `data/garmin/` i krótkiego podsumowania w `exports/`. Nie zapisuj tokenów w tych katalogach.
5. Wyłącznie metody odczytowe. Nie przesyłaj treningów do zegarka, nie zmieniaj aktywności i nie usuwaj danych.
6. Logowanie w lokalnym terminalu; obsługa wymaganej ponownej autoryzacji. Hasło i tokeny pozostają poza plikami projektu.
7. Możliwość użycia ręcznego eksportu Garmin Connect przy niedziałającym połączeniu. Po imporcie sprawdź kilka wartości z widokiem Garmin Connect.

Nie dodawaj serwera, orkiestratora ani harmonogramu do pierwszego importera. Cykliczne uruchamianie jest późniejszym, oddzielnym etapem.
