---
name: szukaj-produktu
description: Użyj, gdy użytkownik napisze „Szukaj Produktu” albo poprosi o znalezienie produktu do bazy posiłków. Znajdź warianty w uzgodnionych źródłach, pokaż krótką listę do wyboru i dodaj do Google Sheets wyłącznie po zatwierdzeniu.
---

# Szukaj Produktu

Celem jest dodanie wybranego **gotowego produktu** do zakładki „Baza posiłków i produktów” prywatnego Google Sheets „100 days challenge”. Samo wyszukanie nie zmienia arkusza. Użytkownik może wywołać ten skill zwrotem **„Szukaj Produktu”**; jeśli nie poda rodzaju ani nazwy produktu, zapytaj, czego szuka.

## Znajdź i pokaż

1. Sprawdź najpierw bazę, czy produkt i dokładny wariant już istnieją. Jeśli tak, pokaż istniejący wpis i zapytaj, czy szukać innego wariantu.
2. Szukaj przede wszystkim na [Lidl.pl](https://www.lidl.pl/) — to uzgodniona baza produktów. [drLifestyle](https://drlifestyle.pl/?s=Lidl&post_type=post) może podpowiedzieć wariant, lecz wartości odżywcze potwierdź na stronie produktu lub etykiecie. Nie sprawdzaj dostępności w konkretnym sklepie. Jeśli strony są niedostępne lub etykieta nieczytelna, poproś o link albo dane z opakowania; nie zgaduj.
3. Pokaż krótką listę, zwykle 3–5 pasujących wariantów: pełna nazwa/marka, gramatura opakowania, kcal oraz białko, węglowodany, tłuszcz i cukry na **100 g**, link do źródła i jawne braki danych. Nie utożsamiaj wartości na 100 ml z wartościami na 100 g bez wiarygodnego przelicznika. Jeśli wyników jest mniej, pokaż dostępne.
4. Poproś użytkownika o wskazanie wariantu lub wariantów i **wyraźne zatwierdzenie dodania do bazy**. Jeżeli dane odżywcze są niepełne albo szacowane, zaznacz to przed zatwierdzeniem. Dopóki zatwierdzenie nie padnie, nie zapisuj żadnego wiersza.

## Po zatwierdzeniu

1. Odczytaj ponownie nagłówki, używane ID i istniejące wpisy. Przy identycznym wariancie nie twórz duplikatu; powiedz, który wpis już istnieje.
2. Przed edycją utwórz kopię arkusza na Google Drive z datą i godziną Europe/Warsaw. Dodaj tylko zatwierdzone produkty, nadając unikalne ID. Wpisz `Rodzaj = Produkt`, `Porcja odniesienia = 100 g`, dostępne makroskładniki, dokładne źródło i zwięzłe uwagi o brakach lub szacunkach. Pola składników i przepisu zostaw puste. Nie wpisuj zera zamiast braku danych.
3. Odczytaj zapisane wiersze, potwierdź ID, wariant, jednostki i liczby. Nie dodawaj produktu do Planu posiłków, jeśli użytkownik o to nie poprosił. Zwróć link do bazy i krótkie potwierdzenie.

Stosuj zasady prywatności, backupu i formatowania z `AGENTS.md` oraz reguły żywienia z `RULES.md`.
