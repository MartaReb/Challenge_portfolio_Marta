# Challenge_portfolio_Marta

# TASK 1
## Subtask 1
10/10 punktów :blush:

## Subtask 3
Cześć! Mam na imię Marta 🙂 Jakiś czas temu postanowiłam się przebranżowić i zostać testerką oprogramowania. Od tego czasu staram się zdobywać wiedzę w zakresie testowania oraz poszerzać tę już zdobytą. 

Zdecydowałam się na udział w Dare -IT Portfolio Challenge, ponieważ jest to świetna okazja do zdobywania nowych umiejętności oraz poznania ludzi o podobnych celach i zainteresowaniach. W projekcie chciałabym jak najwięcej uczyć się poprzez praktykę: ćwiczyć wykorzystywanie technik testowania, zgłaszanie błędów, korzystanie z narzędzi oraz tworzenie dokumentacji testerskiej. Mam nadzieję, że moja praca zaowocuje zdobyciem pracy jako tester oprogramowania 🙂

## Subtask 4
- Na czym polega ta aplikacja? Do czego służy?

Aplikacja służy do zbierania i zarządzania informacjami o piłkarzach, rozegranych przez nich meczach oraz tworzenia raportów oceniających graczy.

- Jakie funkcjonalności znajdują się w aplikacji? Do czego służą. Czy są intuicyjne, czy może byś coś zmienił_a?
    - Dodawanie nowych graczy (jest jedną z ważniejszych funkcji, nie powinno znajdować się w sekcji “Linki pomocnicze”)
    - Edytowanie informacji o graczach (funkcja nieintuicyjna, brak informacji/oznakowania, że po kliknięciu w użytkownika na liście z piłkarzami, można edytować informacje o nim)
    - Wyszukiwanie graczy
    - Sortowanie listy z piłkarzami
    - Filtrowanie listy z piłkarzami po wybranych kryteriach
    - Zarządzanie wyświetlaniem listy poprzez usuwanie i dodawanie kolumn
    - Drukowanie listy z piłkarzami
    - Pobieranie raportów CSV
    - Dodawanie meczy
    - Edytowanie informacji o meczach
    - Tworzenie raportu do danego meczu (nieintuicyjne tworzenie raportów)
    - Edycja raportów (nieintuicyjne)
    - Informacja o ostatnich aktywnościach na stronie
    - Możliwość skontaktowania się z twórcami strony (nieintuicyjne, link przenosi do strony ze Slackiem zespołu deweloperskiego, który pewnie pracował nad stroną)
    - Zmiana języka PL-EN
    - Możliwość przejścia do strony głównej
    - Wylogowanie z aplikacji
- Oceń interfejs aplikacji (wygląd) – czy Ci się podoba, czy nie?
    - Interfejs aplikacji jest prosty (co jest na plus), niestety niedopracowany. Podoba mi się prosta kolorystyka, która nie odwraca uwagi od funkcji aplikacji. Dobrym pomysłem było wykorzystanie w aplikacji ikon, które sygnalizują co się dzieje pod danym elementem, np. w menu. Strona główna jest jednak do całkowitej przebudowy - zawiera informacje, które raczej nie są potrzebne użytkownikowi (ilości: graczy, meczy, raportów, akcji), natomiast umieszcza jedną z ważniejszych funkcji - “Dodaj gracza” w linkach pomocniczych.
    - Dobrym pomysłem byłoby też zwiększyć czcionkę, a może również kolor opisów pól do wprowadzenia przy dodawaniu/edycji nowego gracza/meczu, ponieważ teraz osoby niedowidzące mogłyby mieć problem z odczytaniem ich.
- Czy aplikacja jest intuicyjna? (Intuicyjna, czyli np. nie masz problemu ze zrozumieniem, co należy kliknąć, żeby wejść do formularza dodawania nowego zawodnika piłki nożnej do systemu).
    - W aplikacji jest wiele miejsc nieintuicyjnych, które należałoby poprawić, bo dotyczą podstawowych funkcji aplikacji (wskazałam najważniejsze powyżej).
    - W kilku miejscach nie ma też zachowanego bliźniaczego schematu działania aplikacji (co może utrudniać korzystanie z niej) np. gracza można zaktualizować poprzez kliknięcie na niego na liście z graczami, natomiast mecze można aktualizować tylko poprzez kliknięcie w ikonę ołówka, a już nie da się poprzez kliknięcie na dany mecz na liście.
- Czy zauważasz jakieś błędy? Albo coś wydaje Ci się błędem? Zapisz swoje przemyślenia w pliku. Tutaj masz na to miejsce, czas i przestrzeń! ;)
    - Nieprawidłowa walidacji pół, które są wymagane do wypełnienia podczas dodawania nowego gracza oraz dodawania meczu (niejasne komunikaty lub ich brak)
    - Brak możliwości usunięcia zawodnika, meczu oraz raportu
    - Podczas dodawania nowego gracza:
        - możliwość dodania zawodników o takich samych danych obligatoryjnych
        - możliwość wpisania nieprawidłowego nr telefonu (w kodzie zamiast type=”text”, można by było użyć w <input> type=”tel”),
        - możliwość wpisania ujemnej lub bardzo dużej wagi oraz wzrostu (brak w <input> max i min wartości ograniczającej wpisywanie danych),
        - możliwość wpisania nieprawidłowej daty urodzin (osoby, która się jeszcze nie urodziła, bądź nie jest możliwe, żeby jeszcze żyła),
        - po dodaniu języka lub linka z youtuba dodatkowo wyświetla się pole na kolejny język/kolejny link
        - w polu “Link do Youtub” oraz “Profil facebook” można wpisać dowolne znaki, mimo, że raczej powinny to być tylko linki do stron (podobnie z polami: “Łączy nas piłka” i “90 minut” jeżeli pola te miałyby być miejscem na linki do profilów zawodników na tych stronach/informacji o meczach)
        - brak ograniczenia wpisywania ilości znaków w polach (pojawiający się zbyt długi tekst, może utrudniać przeglądanie listy)
    - Podczas dodawania nowego meczu:
        - w polach “Zdobyte gole” i “Stracone gole” brak ograniczenia we wpisaniu górnej granicy liczby goli
        - możliwość wpisania liczby ujemnej lub nieskończenie dużej dla pól “Czas gry” i “Numer” (brak w <input> max i min wartości ograniczającej wpisywanie danych)
    - Podczas tworzenia i edycji raportów:
        - możliwość robienia kilku raportów dla jednego gracza do jednego meczu
        - raport zapisuje się mimo, że nie klikamy w przycisk “Save”
        - aby dodać nowy raport trzeba uzupełnić informacje o województwie w profilu gracza (nie ma o tym informacji przy dodawaniu gracza)
        - kliknięcie w link [www.futbolkolektyw.pl](http://www.futbolkolektyw.pl) znajdujący się w stopce raportu powoduje wywołanie błędu 404
        - liczbę przyznanych “gwiazdek” można edytować tylko w połowie raportu, mimo, że “gwiazdki” widać od razu na górze raportu (nieintuicyjna funkcja)
        - brak wyjaśnienia (brak tooltipów) dostępnych akcji w funkcji “Rozpocznij mecz”
    - Lista z graczami:
        - sortowanie: nieprawidłowe sortowanie alfabetyczne informacji w kolumnach “Imię”, “Nazwisko”, “Pozycja” i “Klub” na liście z graczami
        - sortowanie: brak możliwości sortowania po kolumnach “Mecze” i “Raporty” na liście z graczami
        - filtrowanie: nieprawidłowe filtrowanie wg parametrów max i min wiek
        - filtrowanie: zresetowanie wpisanych wcześniej filtrów nie powoduje, że pojawia się cała lista z graczami
        - brak możliwości usunięcia zapisanych wcześniej informacji, bez dodania nowych (zostawienie pustego pola) - informacje o graczu nie zapisują się mimo komunikatu “Zapisano gracza”, na stronie głównej pokazuje się też informacja, że zawodnik został zaktualizowana, a nie miało to miejsca
        - możliwość wydrukowania informacji o zawodnikach, którzy znajdują się tylko na wyświetlanej w danym momencie stronie listy (czyli maksymalnie 10 zawodników)
        - możliwość wygenerowania raportu CSV tylko z zawodnikami, którzy wyświetlają się na danej stronie listy (maks. 10 zawodników)
        - w wygenerowanym raporcie CSV w kolumnie “Wiek” wyświetla się data urodzenia oraz zamiast ilości rozegranych meczy oraz stworzonych raportów wyświetlają się napisy “[object Object]”
        - wchodząc w informacje o konkretnym piłkarzu - wchodzimy od razu w tryb edycji
    - Brak możliwości sortowania listy z meczami i raportami
    - Angielskie nazwy przycisków (”Submit”, “Clear”, “Save”), angielskie opisy pól (”General”, “Web match”, “Filters”, “Age”, “Reset”, “Rate”, “Sort”, “Print”, “Download CSV”, “Print”, “View Columns”, “Filter Table” ) oraz angielskie komunikaty (”Sorry, no matching records found”) w polskiej wersji językowej strony
    - Literówka: “Aktywnosć” zamiast “Aktywność” na stronie głównej
    - Słabo widoczne lub niewidoczne paski do przewijania strony
