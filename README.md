# Challenge_portfolio_Marta

# TASK 1
## Subtask 1
10/10 punktów :blush:

## Subtask 3
Cześć! Mam na imię Marta 🙂 Jakiś czas temu postanowiłam się przebranżowić i zostać testerką oprogramowania. Od tego czasu konsekwentnie staram się zdobywać nową wiedzę w zakresie testowania oraz poszerzać tę już zdobytą. 

Zdecydowałam się na udział w Dare-IT Portfolio Challenge, ponieważ jest to świetna okazja do zdobywania nowych umiejętności oraz poznania ludzi o podobnych celach i zainteresowaniach. W projekcie chciałabym jak najwięcej uczyć się poprzez praktykę: ćwiczyć wykorzystywanie technik testowania, zgłaszanie błędów, korzystanie z narzędzi oraz tworzenie dokumentacji testerskiej. Mam nadzieję, że moje wysiłki zaowocują zdobyciem pracy jako tester oprogramowania 🙂

## Subtask 4
- Na czym polega ta aplikacja? Do czego służy?

Aplikacja służy do zbierania i zarządzania informacjami o piłkarzach, rozegranych przez nich meczach oraz tworzenia raportów oceniających graczy.

- Jakie funkcjonalności znajdują się w aplikacji? Do czego służą. Czy są intuicyjne, czy może byś coś zmienił_a?
    - Dodawanie nowych graczy (jest jedną z ważniejszych funkcji, nie powinno znajdować się w sekcji “Linki pomocnicze”)
    - Edytowanie informacji o graczach (funkcja nieintuicyjna, brak informacji/oznakowania, że po kliknięciu w zawodnika na liście z piłkarzami, można edytować informacje o nim)
    - Wyszukiwanie graczy
    - Sortowanie listy z piłkarzami
    - Filtrowanie listy z piłkarzami po wybranych kryteriach
    - Zarządzanie wyglądem listy poprzez usuwanie i dodawanie kolumn
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
    
- Oceń interfejs aplikacji.
    - Interfejs aplikacji jest prosty (co jest na plus), niestety niedopracowany. Podoba mi się prosta kolorystyka, która nie odwraca uwagi od funkcji aplikacji. Dobrym pomysłem było wykorzystanie w aplikacji ikon, które sygnalizują co się dzieje pod danym elementem, np. w menu. Strona główna jest jednak do całkowitej przebudowy - zawiera informacje, które raczej nie są potrzebne użytkownikowi (ilości: graczy, meczy, raportów, akcji), natomiast umieszcza jedną z ważniejszych funkcji - “Dodaj gracza” w linkach pomocniczych.
    - Dobrym pomysłem byłoby też zwiększenie czcionki, a może również zmiana koloru opisów pól przy dodawaniu/edycji nowego gracza/meczu, ponieważ w aktualnej wersji mogą być nieczytelne dla osób niedowidzących.
   
- Czy aplikacja jest intuicyjna?
    - W aplikacji jest wiele miejsc nieintuicyjnych, które należałoby poprawić, bo dotyczą podstawowych funkcji aplikacji (wskazałam najważniejsze powyżej).
    - W kilku miejscach nie ma też zachowanego bliźniaczego schematu działania aplikacji (co może utrudniać korzystanie z niej) np. gracza można zaktualizować poprzez kliknięcie na niego na liście z graczami, natomiast mecze można aktualizować tylko poprzez kliknięcie w ikonę ołówka.
   
- Czy zauważasz jakieś błędy? Albo coś wydaje Ci się błędem?
    - Nieprawidłowa walidacja pól, które są wymagane do wypełnienia podczas dodawania nowego gracza oraz dodawania meczu (niejasne komunikaty lub ich brak)
    - Brak możliwości usunięcia zawodnika, meczu oraz raportu
    - Podczas dodawania nowego gracza:
        - możliwość dodania zawodników o takich samych danych obligatoryjnych,
        - możliwość wpisania nieprawidłowego nr telefonu (w kodzie zamiast type=”text”, można by było użyć w <input> type=”tel”),
        - możliwość wpisania ujemnej lub bardzo dużej wagi oraz wzrostu (brak w <input> max i min wartości ograniczającej wpisywanie danych),
        - możliwość wpisania nieprawidłowej daty urodzin (osoby, która się jeszcze nie urodziła, bądź nie jest możliwe, żeby jeszcze żyła),
        - w polu “Link do Youtube” oraz “Profil facebook” można wpisać dowolne znaki, mimo że raczej powinny to być tylko linki do stron (podobnie z polami: “Łączy nas piłka” i “90 minut” jeżeli pola te miałyby być miejscem na linki do profilów zawodników na tych stronach/informacji o meczach)
        - brak ograniczenia wpisywania ilości znaków w polach (pojawiający się zbyt długi tekst, może utrudniać przeglądanie listy)
    - Podczas dodawania nowego meczu:
        - możliwość wpisania liczby ujemnej lub dowolnie dużej dla pól “Czas gry” i “Numer” (brak w <input> max i min wartości ograniczającej wpisywanie danych)
    - Podczas tworzenia i edycji raportów:
        - możliwość robienia kilku raportów dla jednego gracza do jednego meczu
        - raport zapisuje się mimo, że nie klikamy w przycisk “Save”
        - aby dodać nowy raport trzeba uzupełnić informacje o województwie w profilu gracza (nie ma o tym informacji przy dodawaniu gracza)
        - kliknięcie w link [www.futbolkolektyw.pl](http://www.futbolkolektyw.pl) znajdujący się w stopce raportu powoduje wywołanie błędu 404
        - liczbę przyznanych “gwiazdek” można edytować tylko w połowie raportu, mimo że “gwiazdki” widać od razu na górze raportu (nieintuicyjna funkcja)
        - brak wyjaśnienia (brak tooltipów) dostępnych akcji w funkcji “Rozpocznij mecz”
    - Lista z graczami:
        - sortowanie: nieprawidłowe sortowanie alfabetyczne informacji w kolumnach “Imię”, “Nazwisko”, “Pozycja” i “Klub” na liście z graczami
        - sortowanie: brak możliwości sortowania po kolumnach “Mecze” i “Raporty” na liście z graczami
        - filtrowanie: nieprawidłowe filtrowanie wg parametrów max i min wiek
        - filtrowanie: zresetowanie wpisanych wcześniej filtrów nie powoduje, że pojawia się cała lista z graczami
        - brak możliwości usunięcia zapisanych wcześniej informacji, bez dodania nowych (zostawienie pustego pola) - informacje o graczu nie zapisują się mimo komunikatu “Zapisano gracza”, na stronie głównej pokazuje się też błędna informacja, że zawodnik został zaktualizowany,
        - możliwość wydrukowania informacji o zawodnikach, którzy znajdują się tylko na wyświetlanej w danym momencie stronie listy (czyli maksymalnie 10 zawodników)
        - możliwość wygenerowania raportu CSV tylko z zawodnikami, którzy wyświetlają się na danej stronie listy (maks. 10 zawodników)
        - w wygenerowanym raporcie CSV w kolumnie “Wiek” wyświetla się data urodzenia, a zamiast ilości rozegranych meczy oraz stworzonych raportów wyświetlają się napisy “[object Object]”
        - wchodząc w informacje o konkretnym piłkarzu - wchodzimy od razu w tryb edycji
    - Brak możliwości sortowania listy z meczami i raportami
    - Angielskie nazwy przycisków (”Submit”, “Clear”, “Save”), angielskie opisy pól (”General”, “Web match”, “Filters”, “Age”, “Reset”, “Rate”, “Sort”, “Print”, “Download CSV”, “Print”, “View Columns”, “Filter Table” ) oraz angielskie komunikaty (”Sorry, no matching records found”) w polskiej wersji językowej strony
    - Literówka: “Aktywnosć” zamiast “Aktywność” na stronie głównej
    - Słabo widoczne lub niewidoczne paski do przewijania strony
   
   
 # TASK 2
 ## Subtask 1 
 **Przypadki testowe dla polskiej wersji aplikacji Scouts Panel napisane na podstawie User Story** 
 
 👉 https://docs.google.com/document/d/1mK37GsoEOsTZ10nhPyoEjv-YgcUICoEXTmWwzlLapzk/edit
 
 ## Subtask 2 
 **Przypadki testowe dla polskiej wersji aplikacji Scouts Panel napisane na podstawie “własnych doświadczeń"**
 
 👉 https://docs.google.com/document/d/1xkZTpiF0Zz2_4DDGyjX7VrOgu4zt_uVUMsjPm1rWedk/edit
 
 ## Subtask 3 
 **Po co piszemy test case’y?**
 - Przypadki testowe pozwalają nam uporządkować sposób testowania oprogramowania krok po kroku.
 - Dobre pokrycie oprogramowania przypadkami testowymi daje nam pewność, że podczas testów nie pominęliśmy żadnej ważnej funkcjonalności.
 - Na podstawie przypadków testowych można przygotować metryki pokazujące, np. liczbę planowanych i wykonanych przypadków testowych, liczbę tych, które zakończyły się sukcesem, i tych, które wykazały błędy, a później przedstawić to w raporcie z testów.
 - Tworząc przypadki testowe, możemy zauważyć braki danych oraz problemy z logiką oprogramowania.
 - Jest to też forma spisania wiedzy o testowanym oprogramowaniu, która może przydać się przy wprowadzaniu do zespołu nowej osoby.
 - To dokumentacja pracy testera.
 - Można wykorzystać przypadki testowe w kontekście testów akceptacyjnych w celu potwierdzenia działania aplikacji zgodnie z oczekiwaniami.
 - Spisane przypadki testowe, mogą stanowić scenariusze do oskryptowania i przeprowadzenia testów automatycznych.
 
 ## Subtask 4 
 **Przypadki testowe dla polskiej wersji aplikacji Pick Eat Up napisane na podstawie “własnych doświadczeń"**
 
👉 https://docs.google.com/document/d/164lum8wfixR88mhimARGnkl_FtmL5E5n7eGDKlgOF60/edit?usp=sharing

# TASK 3
## Subtask 1 
**Zgłoszania błędów znalezionych w polskiej wersji aplikacji Scouts Panel**

👉 https://drive.google.com/drive/folders/1aorSgvEQ9CEgaeT7lzUkt_orGRwpoZUz

## Subtask 3 
**Raport z testów aplikacji Scouts Panel**

👉 https://drive.google.com/drive/folders/1aorSgvEQ9CEgaeT7lzUkt_orGRwpoZUz
