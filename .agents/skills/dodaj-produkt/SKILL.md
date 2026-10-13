---
name: dodaj-produkt
description: Użyj, gdy użytkownik napisze „Dodaj Produkt” i poda zdjęcie etykiety, opis lub link do gotowego produktu albo posiłku NTFY. Sprawdź wariant i makroskładniki, a następnie dodaj wpis do bazy Google Sheets bez ponownego pytania o zgodę, jeśli dane wystarczają.
---

# Dodaj Produkt

Wywołanie **„Dodaj Produkt”** z materiałem od użytkownika jest zleceniem dodania do „Bazy posiłków i produktów” w prywatnym Google Sheets „100 days challenge”. Nie wymagaj drugiego zatwierdzenia. Jeśli brak danych uniemożliwia identyfikację produktu lub wiarygodne ustalenie kcal, białka, węglowodanów i tłuszczu, zapytaj o brakujące informacje przed zapisem.

1. Odczytaj ze zdjęcia, opisu lub linku markę, pełną nazwę, smak/wariant, gramaturę opakowania lub posiłku, wielkość porcji i wartości odżywcze. Nie dopowiadaj nieczytelnych cyfr. Sprawdź dokładny wariant na [Lidl.pl](https://www.lidl.pl/) lub w etykiecie przekazanej przez użytkownika; [drLifestyle](https://drlifestyle.pl/?s=Lidl&post_type=post) może pomóc rozpoznać produkt, lecz nie zastępuje etykiety. Nie sprawdzaj lokalnej dostępności.
2. Ujednolić jednostki: zwykły gotowy produkt zapisuj jako `Rodzaj = Produkt`, na `100 g`; posiłek cateringowy NTFY jako `Rodzaj = NTFY`, na `1 posiłek`. Przelicz wartości z porcji tylko gdy znana jest jej masa. Nie zamieniaj 100 ml na 100 g bez wiarygodnego przelicznika. Cukry są częścią węglowodanów; brak cukrów pozostaw pusty.
3. Zweryfikuj kcal i makroskładniki z właściwą etykietą oraz sprawdź ich jednostki i podstawową spójność. Różnicy wobec rachunku 4/4/9 nie „poprawiaj” automatycznie: może wynikać m.in. z zaokrągleń lub błonnika. Gdy dwa źródła dla rzekomo tego samego wariantu są sprzeczne, wyjaśnij różnicę z użytkownikiem. Nie zapisuj niezweryfikowanych podstawowych makroskładników jako faktów.
4. Odczytaj bazę i sprawdź, czy identyczny wariant już istnieje. Jeśli tak, podaj ID i nie dodawaj duplikatu. W przeciwnym razie odczytaj nagłówki, używane ID i docelowy zakres, utwórz kopię arkusza na Google Drive z datą i godziną Europe/Warsaw, a potem dodaj jeden wiersz z unikalnym ID, porcją, wartościami, źródłem i krótką uwagą o brakach. Składniki i przepis zostaw puste.
5. Odczytaj zapisany wiersz i sprawdź nazwę, jednostki, kcal oraz makroskładniki. W odpowiedzi podaj ID, zweryfikowane wartości i źródło. Nie dodawaj produktu do Planu posiłków, jeśli użytkownik tego nie zlecił.

Stosuj zasady prywatności i edycji arkusza z `AGENTS.md`. Zdjęcia etykiet i dane użytkownika nie trafiają do publicznego repozytorium.
