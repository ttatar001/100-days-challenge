# Przyszła integracja Garmina

Zegarek jest obecnie w reklamacji; integracja nie działa. Po jego powrocie przygotuj prosty, uruchamiany ręcznie importer odczytowy z aktualną wersją [`python-garminconnect`](https://github.com/cyberjunky/python-garminconnect). Przed implementacją sprawdź bieżące API i sposób logowania. Pobieraj aktywności, czas, dystans, dostępne tętno i kalorie, kroki oraz dobowe podsumowania. Dla siłowni nie dopowiadaj nieznanych ćwiczeń i ciężarów. Rozróżniaj kalorie aktywne i całkowite, braki danych i rzeczywiste zera; nie doliczaj ponownie treningu do całkowitego wydatku.

Logowanie i tokeny przechowuj wyłącznie poza repozytorium. Importer nie może zmieniać ani usuwać danych Garmina. Przy pierwszym uruchomieniu porównaj kilka odczytów z Garmin Connect. Ręczny eksport może być wariantem awaryjnym. Nie dodawaj harmonogramu ani serwera do pierwszej wersji.
