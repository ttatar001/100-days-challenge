---
name: dodaj-przepis
description: Użyj, gdy użytkownik napisze „Dodaj Przepis” i poda zdjęcie, opis lub link do dania do przygotowania. Sprawdź składniki, policz makroskładniki na posiłek i dodaj przepis do bazy Google Sheets bez ponownego pytania o zgodę, jeśli dane wystarczają.
---

# Dodaj Przepis

Wywołanie **„Dodaj Przepis”** z materiałem od użytkownika jest zleceniem dodania dania do „Bazy posiłków i produktów” w prywatnym Google Sheets „100 days challenge”. Nie wymagaj drugiego zatwierdzenia. Jeśli nie da się wiarygodnie ustalić składników, ich ilości, liczby porcji albo podstawowych makroskładników, zapytaj o brakujące informacje przed zapisem.

1. Odczytaj zdjęcie, opis lub podany link. Ustal nazwę, składniki z ilościami, liczbę porcji i sposób przygotowania. Jeżeli przepis pochodzi z sieci, sprawdź oryginał w [Kuchni Lidla — lekkie i fit](https://kuchnialidla.pl/przepisy/lekkie-i-fit) lub rzeczywisty przepis na [drLifestyle](https://drlifestyle.pl/?s=Lidl&post_type=post). Nie zamieniaj wariantu użytkownika na podobny przepis bez jego wiedzy.
2. Oblicz kcal, białko, węglowodany, tłuszcz i dostępne cukry z **jadalnych ilości wszystkich składników**, także tłuszczu użytego do przygotowania. Dla składników markowych korzystaj z dokładnych etykiet użytkownika albo danych produktu na [Lidl.pl](https://www.lidl.pl/); dla podstawowych składników bez etykiety użyj wiarygodnej tabeli składu żywności, np. [USDA FoodData Central](https://fdc.nal.usda.gov/), z właściwą postacią surową lub po obróbce. Wynik całego przepisu podziel przez rzeczywistą liczbę porcji. Zapisz źródła obliczeń i oznacz szacunki; nie zgaduj pominiętej gramatury ani nie podawaj pozornej dokładności. Jeśli brakuje podstawowych danych do rachunku, zapytaj przed dodaniem.
3. Odczytaj bazę i sprawdź, czy identyczna receptura już istnieje. Jeśli tak, podaj ID i nie dodawaj duplikatu; istotnie zmienione składniki lub proporcje to osobny wariant.
4. Odczytaj nagłówki, używane ID i docelowy zakres. Utwórz kopię arkusza na Google Drive z datą i godziną Europe/Warsaw. Dodaj jeden wiersz z unikalnym ID, `Rodzaj = Do przygotowania`, `Porcja odniesienia = 1 posiłek`, makroskładnikami na tę porcję, składnikami z gramaturą, źródłem i uwagą o metodzie obliczenia. Przepis zapisz własnymi słowami, z każdym krokiem w nowej linii; nie kopiuj całego tekstu strony. Brak cukrów pozostaw pusty, nie wpisuj zera.
5. Odczytaj zapisany wiersz i sprawdź porcję, sumy oraz podział kroków. W odpowiedzi podaj ID, składniki i wartości na 1 posiłek, źródła oraz ewentualne szacunki. Nie dodawaj dania do Planu posiłków, jeśli użytkownik tego nie zlecił.

Stosuj zasady prywatności i edycji arkusza z `AGENTS.md`. Zdjęcia i dane użytkownika nie trafiają do publicznego repozytorium.
