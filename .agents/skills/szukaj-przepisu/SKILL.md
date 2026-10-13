---
name: szukaj-przepisu
description: Użyj, gdy użytkownik napisze „Szukaj Przepisu” albo poprosi o przepis do bazy posiłków. Znajdź konkretny przepis w uzgodnionych źródłach, przedstaw składniki, kroki i makroskładniki, a do Google Sheets dodaj dopiero po zatwierdzeniu.
---

# Szukaj Przepisu

Celem jest dodanie zatwierdzonego dania **do przygotowania** do zakładki „Baza posiłków i produktów” prywatnego Google Sheets „100 days challenge”. Użytkownik może wywołać ten skill zwrotem **„Szukaj Przepisu”**. Jeśli nie poda rodzaju dania, składnika lub okazji, zapytaj o jedną z tych wskazówek.

## Znajdź i pokaż

1. Sprawdź bazę, czy danie lub ten sam przepis już istnieje. Jeśli istnieje, pokaż wpis i poszukaj innego przepisu tylko gdy użytkownik tego chce.
2. Szukaj przede wszystkim w [Kuchni Lidla — lekkie i fit](https://kuchnialidla.pl/przepisy/lekkie-i-fit), ze szczególną uwagą na przepisy Kingi Paruzel. Możesz korzystać z [drLifestyle](https://drlifestyle.pl/?s=Lidl&post_type=post), jeśli dany artykuł zawiera rzeczywisty przepis. [Lidl.pl](https://www.lidl.pl/) służy do sprawdzania produktów i ich etykiet. Nie sprawdzaj dostępności w konkretnym sklepie. Jeśli źródła nie są dostępne, poproś o link; nie wymyślaj przepisu ani wartości.
3. Pokaż **jeden konkretny przepis**: nazwę i link, liczbę porcji, składniki z gramaturą na cały przepis i na 1 posiłek, czas przygotowania, kroki własnymi słowami (każdy w nowej linii) oraz kcal, białko, węglowodany, tłuszcz i cukry na 1 posiłek. Oblicz wartości z danych źródłowych lub etykiet składników. Oznacz szacunki i braki; nie podawaj pozornej dokładności. Gdy ilości składników nie pozwalają na wiarygodne wyliczenie, wyjaśnij, jakich danych brakuje.
4. Zapytaj, czy użytkownik **zatwierdza dokładnie tę wersję przepisu i dodanie jej do bazy**. Jeśli zmieni składnik, porcję lub sposób przygotowania, przelicz propozycję i pokaż ją ponownie. Przed zatwierdzeniem nie zapisuj wiersza.

## Po zatwierdzeniu

1. Odczytaj ponownie nagłówki, używane ID i istniejące przepisy. Nie dodawaj duplikatu; różniącą się recepturę zapisz jako osobny wariant.
2. Przed edycją utwórz kopię arkusza na Google Drive z datą i godziną Europe/Warsaw. Dodaj zatwierdzony wpis z unikalnym ID, `Rodzaj = Do przygotowania`, `Porcja odniesienia = 1 posiłek`, makroskładnikami, składnikami z ilościami, przepisem z każdym krokiem w nowej linii, linkiem do źródła i krótką uwagą o obliczeniach lub brakach. Nie wpisuj zera zamiast braku danych. Opisz przygotowanie własnymi słowami, nie kopiuj pełnego tekstu strony.
3. Odczytaj zapisany wiersz i sprawdź ID, porcję, liczby, składniki i podział kroków. Nie dodawaj przepisu do Planu posiłków, jeśli użytkownik o to nie poprosił. Zwróć link do bazy i krótkie potwierdzenie.

Stosuj zasady prywatności, backupu i formatowania z `AGENTS.md` oraz reguły żywienia z `RULES.md`.
