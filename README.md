# Challenge_portfolio_Marta

# TASK 1
## Subtask 1
10/10 punktów :blush:

## Subtask 3

Cześć! Mam na imię Marta 🙂 Jakiś czas temu postanowiłam się przebranżowić i zostać testerką oprogramowania. Od tego czasu konsekwentnie staram się zdobywać nową wiedzę w zakresie testowania oraz poszerzać tę już zdobytą. 

Zdecydowałam się na udział w Dare-IT Portfolio Challenge, ponieważ jest to świetna okazja do zdobywania nowych umiejętności oraz poznania ludzi o podobnych celach i zainteresowaniach. W projekcie chciałabym jak najwięcej uczyć się poprzez praktykę: ćwiczyć wykorzystywanie technik testowania, zgłaszanie błędów, korzystanie z narzędzi oraz tworzenie dokumentacji testerskiej. Mam nadzieję, że moje wysiłki zaowocują zdobyciem pracy jako tester oprogramowania 🙂


<p align="center">
  <img src="https://user-images.githubusercontent.com/49365894/205621838-e29e13e1-e031-4ed9-80ec-b67662cc7c2d.jpg">
</p>

źródło: https://pixabay.com/ -|

## Subtask 4
1. Na czym polega ta aplikacja? Do czego służy?

    Aplikacja służy do zbierania i zarządzania informacjami o piłkarzach, rozegranych przez nich meczach oraz tworzenia raportów oceniających graczy.

2. Jakie funkcjonalności znajdują się w aplikacji? Do czego służą. Czy są intuicyjne, czy może byś coś zmienił_a?
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
    
3. Oceń interfejs aplikacji.
    - Interfejs aplikacji jest prosty (co jest na plus), niestety niedopracowany. Podoba mi się prosta kolorystyka, która nie odwraca uwagi od funkcji aplikacji. Dobrym pomysłem było wykorzystanie w aplikacji ikon, które sygnalizują co się dzieje pod danym elementem, np. w menu. Strona główna jest jednak do całkowitej przebudowy - zawiera informacje, które raczej nie są potrzebne użytkownikowi (ilości: graczy, meczy, raportów, akcji), natomiast umieszcza jedną z ważniejszych funkcji - “Dodaj gracza” w linkach pomocniczych.
    - Dobrym pomysłem byłoby też zwiększenie czcionki, a może również zmiana koloru opisów pól przy dodawaniu/edycji nowego gracza/meczu, ponieważ w aktualnej wersji mogą być nieczytelne dla osób niedowidzących.
   
4. Czy aplikacja jest intuicyjna?
    - W aplikacji jest wiele miejsc nieintuicyjnych, które należałoby poprawić, bo dotyczą podstawowych funkcji aplikacji (wskazałam najważniejsze powyżej).
    - W kilku miejscach nie ma też zachowanego bliźniaczego schematu działania aplikacji (co może utrudniać korzystanie z niej) np. gracza można zaktualizować poprzez kliknięcie na niego na liście z graczami, natomiast mecze można aktualizować tylko poprzez kliknięcie w ikonę ołówka.
   
5. Czy zauważasz jakieś błędy? Albo coś wydaje Ci się błędem?
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
 👉 [Przypadki testowe dla polskiej wersji aplikacji Scouts Panel napisane na podstawie User Story](https://docs.google.com/spreadsheets/d/1SP-CrVc0SAjelZIyhspTlQ3_JZOpGMnU5815dC1lqvA/edit#gid=0)
 
 ## Subtask 2 
 👉 [Przypadki testowe dla polskiej wersji aplikacji Scouts Panel napisane na podstawie “własnych doświadczeń"](https://docs.google.com/spreadsheets/d/1zTbFyk3hQX7hQHB8TF2cweT7H1wb_Au-MV93QLbg09M/edit#gid=0)
 
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
 👉 [Przypadki testowe dla polskiej wersji aplikacji Pick Eat Up napisane na podstawie “własnych doświadczeń"](https://docs.google.com/document/d/164lum8wfixR88mhimARGnkl_FtmL5E5n7eGDKlgOF60/edit?usp=sharing)
 
# TASK 3
## Subtask 1 
👉 [Zgłoszania błędów znalezionych w polskiej wersji aplikacji Scouts Panel](https://docs.google.com/document/d/1dSYjm6jRazSG24NIZUPnGj1uk4Ty9UbkomDj8_uM5wg/edit)

## Subtask 3 
👉 [Raport z testów aplikacji Scouts Panel](https://docs.google.com/document/d/1keU7FVRSoz-UN3lHbbZEwY4mohcVX0SaG0G32xQ7nj4/edit)

# TASK 4
## Subtask 1
👉 [Zgłoszenia błędów dla aplikacji mobilnej Focusly](https://docs.google.com/spreadsheets/d/1nip9iNvL0U9zRAD8Nrj2_VwPruIk00vqF09xSwV-fKI/edit#gid=0)

## Subtask 3
**1. Do czego służy ta aplikacja? Jaki jest cel tej aplikacji?**
    
📝 Aplikacja służy do zarabiania na sprzedawaniu dostępu do wszystkich funkcjonalności i nagrań w aplikacji w trybie miesięcznym lub rocznym.
    
**2. Kto ma być użytkownikiem końcowym aplikacji?**

📝 Użytkownikiem końcowym mają być osoby, które chcą poprawić swój dobrostan psychiczny lub chcące zredukować stres poprzez np. medytacje, techniki relaksacyjne, techniki oddechowe, itp.
    
**3. Czy według Ciebie aplikacja jest user friendly?**

📝 Uważam, że potrzeba by było kilka zmian, żeby aplikacja ta stała się user-friendly. Jest kilka miejsc, które nie są intuicyjne i mogą spowodować, że użytkownik może się poczuć zagubiony i zrezygnuje z korzystania z niej. Można takie miejsca znaleźć już na stronie głównej, korzystając z dostępnych tam funkcji, a przecież strona główna jest wizytówką aplikacji. Niektóre przydatne funkcje w aplikacji są za mało widoczne, podczas gdy inne są zbyt wyeksponowane. Także tekst z opisami w niektórych miejscach mógłby być większy, ponieważ zbyt mały może utrudniać osobom gorzej widzącym przeczytanie informacji.

**4. Jak byś usprawnił aplikację? Co byś w niej poprawił. Czy masz jakiś pomysł na dodatkową funkcjonalność?**

📝 Poprawiłabym aplikacje poprzez:
- Dodanie samouczka,  który po pierwszym uruchomieniu aplikacji podpowiedziałby jak aplikacja działa, gdzie są jej podstawowe funkcje i jak je uruchomić i wyłączyć. Użytkownik sam metodą prób i błędów musi poznawać aplikacje, jeżeli chce z niej korzystać, co może być zniechęcające dla osób, które nie miały z takim rodzajem aplikacji do czynienia.
- Dodanie możliwości przejścia z każdej strony do sekcji z możliwością uzyskania pomocy czy kontaktu z twórcami aplikacji. W tym momencie funkcja ta nie jest łatwo dostępna i trzeba wykonać kilka kroków z głównego menu, żeby do niej dotrzeć.
- Dodanie komunikatów, że jakaś akcja się powiodła, np. założenie konta czy usunięcie konta.
- Zwiększenie czcionki w opisach niektórych elementów.

📝 Pomysły na dodatkowe funkcjonalności:
- Dodanie kalendarz z informacjami kiedy, np. medytowaliśmy.
- Dodanie miejsce na notatki, przemyślenia po wysłuchaniu konkretnych lekcji, miejsce na notatki połączyłabym z kalendarzem.

**5. Jakie dostrzegasz różnice pomiędzy testowaniem aplikacji internetowej, a natywnej?**

📝 Aplikacje internetową trzeba przetestować biorąc pod uwagę przeglądarki internetowe i urządzeniach, natomiast w natywnej możemy się ograniczyć testy do urządzeń z danym systemem operacyjnym. W aplikacji natywnej trzeba zwracać uwagę na odpowiednie rozmieszczenie i wielkość przycisków, czy można przesuwać strony bez klikania w ekran, czy wszystko płynnie można przesuwać i nic się nie zacina. Trzeba też wykonać testy pod względem wysyłanych przez aplikację natywną powiadomień oraz współgranie z panelem nawigacyjnym telefonu. Należy przetestować też wykorzystanie przez aplikację natywną wbudowanych zasobów urządzenia: lokalizacji, aparatu, książki adresowej itp. Powinno się sprawdzić też jak aplikacja natywna zachowa się w przypadku zakłóceń, takich jak połączenia telefoniczne, SMS-y i wiadomości, powiadomienia push itp. a także jak aplikacja zachowuje się w trybie offline. W przypadku aplikacji internetowych warto zwrócić uwagę na to jak dużo danych pobiera z serwera, czy nie przeciąża telefonu, czy jak zachowuje się w warunkach ograniczonego dostępu do internetu.

## Subtask 4
👉 [Zgłoszenia błędów dla aplikacji mobilnej SwipeTo w Jira](https://testerzy.atlassian.net/jira/your-work)

# TASK 5
## Subtask 1
Operatory/zapytania w języku SQL, których się nauczyłam: 

- ❔ SELECT, DISTINCT, AS, UPPER, LOWER, COUNT, SUM, MIN, MAX, AVG,
- ❓ ORDER BY, ASC, DESC, 
- ❔ WHERE, BETWEEN, LIKE, AND, OR, IS (NOT) NULL, IN,
- ❓ LIMIT,
- ❔ GROUP BY,
- ❓ INNER JOIN, LEFT JOIN, RIGHT JOIN, FULL JOIN,
- ❔ CREATE, INSERT, UPDATE,
- ❓ DROP, DELETE,

## Subtask 3 
💡 1. Wyświetl tabelę 'actors' w kolejności alfabetycznej sortując po kolumnie 'surname'.

```sql
SELECT * FROM actors
ORDER BY surname ASC;
```

![1](https://user-images.githubusercontent.com/49365894/204601342-3d58ebc1-ea5b-4701-8abc-e5aaf637bab6.png)


💡 2. Wyświetl film, który powstał w 2019 roku.

```sql
SELECT * FROM movies
WHERE year_of_production = 2019;
```

![2](https://user-images.githubusercontent.com/49365894/204598303-5bccfd6e-49d5-4f50-8376-7d515c66d439.png)


💡 3. Wyświetl wszystkie filmy, które powstały między 1900, a 1999 rokiem.

```sql
SELECT * FROM movies
WHERE year_of_production BETWEEN 1900 AND 1999;
```

![3](https://user-images.githubusercontent.com/49365894/204598350-6dd35c0b-1fd1-44e3-89dd-be888bb0b5e2.png)


💡 4. Wyświetl JEDYNIE tytuł i cenę filmów, które kosztują poniżej 7$.

```sql
SELECT title, price FROM movies
WHERE price < 7;
```

![4](https://user-images.githubusercontent.com/49365894/204598430-411a724e-3ff3-45d2-978c-3bcace5d094c.png)


💡 5. Użyj operatora logicznego AND, aby wyświetlić aktorów o actor_id pomiędzy 4-7 (4 i 7 powinny się wyświetlać). NIE UŻYWAJ operatora BETWEEN.

```sql
SELECT * FROM actors
WHERE actor_id >= 4 AND actor_id <= 7;
```

![5](https://user-images.githubusercontent.com/49365894/204598486-1aa98e25-3b23-4796-8a70-fc6d33831bd9.png)


💡 6. Wyświetl klientów o id 2,4,6 wykorzystaj do tego warunek logiczny. 

```sql
SELECT * FROM customers
WHERE customer_id = 2 OR customer_id = 4 OR customer_id = 6;
```

![6](https://user-images.githubusercontent.com/49365894/204598524-5f9ab4a3-7e27-4fe4-80a3-094bd52ab37b.png)


💡 7. Wyświetl klientów o id 1,3,5 wykorzystaj do tego operator IN. 

```sql
SELECT * FROM customers
WHERE customer_id IN (1,3,5);
```

![7](https://user-images.githubusercontent.com/49365894/204598570-e1b52aa5-3fb9-41ba-97fc-678f46836dc2.png)


💡 8. Wyświetl dane wszystkich osób z tabeli ‘actors’, których imię zaczyna się od ciągu “An”.

```sql
 SELECT * FROM actors
WHERE name LIKE 'An%';
```

![8](https://user-images.githubusercontent.com/49365894/204598622-814551c8-519a-4e6c-95b5-6ef02083fe6b.png)


💡 9. Wyświetl dane klienta, który nie ma podanego adresu email.

```sql
SELECT * FROM customers
WHERE email IS NULL;
```

![9](https://user-images.githubusercontent.com/49365894/204598665-6daa56ba-df75-41fc-b9c3-1abb5cf11b95.png)


💡 10. Wyświetl wszystkie filmy, których cena wynosi powyżej 9$ oraz ich ID mieści się pomiędzy 2 i 8 movie_id.

```sql
SELECT * FROM movies
WHERE (price > 9) AND (movie_id BETWEEN 2 AND 8);
```

![10](https://user-images.githubusercontent.com/49365894/204598731-0c644ed8-a466-474b-a470-be1b201959ca.png)


# TASK 6
## Subtask 1
💡 11. Popełniłam błąd wpisując nazwisko Ani Miler – wpisałam Muler. Znajdź i zastosuj funkcję, która poprawi mój karkołomny błąd 🙈

```sql
UPDATE customers
SET surname = 'Miler'
WHERE customer_id = 3;
```

![11](https://user-images.githubusercontent.com/49365894/205618970-25da5f58-382a-455c-8d79-a22006725019.png)


💡 12. Pobrałam za dużo pieniędzy od klienta, który kupił w ostatnim czasie film o id 4. Korzystając z funkcji join sprawdź, jak ma na imię klient i jakiego ma maila. W celu napisania mu wiadomości o pomyłce fantastycznej szefowej.

```sql
SELECT c.name, c.email
FROM customers AS c
JOIN sale AS s
	ON c.customer_id = s.customer_id
WHERE movie_id = 4;
```

![12](https://user-images.githubusercontent.com/49365894/205619049-1b393d76-c351-49b9-8aeb-7533b1b3ad46.png)


💡 13. Na pewno zauważył_ś, że sprzedawca zapomniał wpisać emaila klientce Patrycji. Uzupełnij ten brak wpisując: [pati@mail.com](mailto:pati@mail.com).

```sql
UPDATE customers
SET email = 'pati@mail.com'
WHERE  customer_id = 4;
```

![13](https://user-images.githubusercontent.com/49365894/205619088-9d6972b8-82e6-4dcf-8259-3e2ab08771b6.png)


💡 14. Dla każdego zakupu wyświetl, imię i nazwisko klienta, który dokonał wypożyczenia oraz tytuł wypożyczonego filmu. (wykorzystaj do tego funkcję inner join, zastanów się wcześniej, które tabele Ci się przydadzą do wykonania ćwiczenia).

```sql
SELECT c.name, c.surname, m.title
FROM customers AS c
JOIN sale AS s
	ON c.customer_id = s.customer_id
JOIN movies AS m
	ON s.movie_id = m.movie_id;
```

![14](https://user-images.githubusercontent.com/49365894/205619192-29956bab-4311-48be-b049-3f228c949de4.png)


💡 15. W celu anonimizacji danych, chcesz stworzyć pseudonimy swoich klientów. - Dodaj kolumnę o nazwie ‘pseudonym’ do tabeli customer,- Wypełnij kolumnę w taki sposób, aby pseudonim stworzył się z dwóch pierwszych liter imienia i ostatniej litery nazwiska. Np. Natalie Pilling → Nag.

```sql
UPDATE customers
SET pseudonim ='Ols'
WHERE customer_id = 1;

UPDATE customers
SET pseudonim ='Kal'
WHERE customer_id = 2;

UPDATE customers
SET pseudonim ='Anr'
WHERE customer_id = 3;

UPDATE customers
SET pseudonim ='Par'
WHERE customer_id = 4;

UPDATE customers
SET pseudonim ='Mao'
WHERE customer_id = 5;

UPDATE customers
SET pseudonim ='Nag'
WHERE customer_id = 6;
```

![15](https://user-images.githubusercontent.com/49365894/205619234-f8bc13ed-0edc-46f7-a872-c2187f1e54c1.png)


💡 16. Wyświetl tytuły filmów, które zostały zakupione, wyświetl tabelę w taki sposób, aby tytuły się nie powtarzały.

```sql
SELECT DISTINCT  m.title
FROM movies AS m
JOIN sale AS s
	ON m.movie_id = s.movie_id;
```

![16](https://user-images.githubusercontent.com/49365894/205619276-ff5466c3-adc2-4b4a-a1b2-79f8fd18fbc2.png)


💡 17. Wyświetl wspólną listę imion wszystkich aktorów i klientów, a wynik uporządkuj alfabetycznie (Wykorzystaj do tego funkcji UNION).

```sql
SELECT name FROM customers
UNION
SELECT name FROM actors
ORDER BY name;
```

![17](https://user-images.githubusercontent.com/49365894/205619297-87e7b674-2e96-4994-b84a-074c36bbc7da.png)


💡 18. Polskę opanowała inflacja i nasz sklepik z filmami również dotknął ten problem. Podnieś cenę wszystkich filmów wyprodukowanych po 2000 roku o 2,5 $ (Pamiętaj, że dolar to domyślna jednostka- nie używaj jej nigdzie).

```sql
UPDATE movies 
SET price = price + 2.5
WHERE year_of_production > 2000;
```

![18](https://user-images.githubusercontent.com/49365894/205619326-03903ee2-8463-4cf9-a5ea-8f812cbf6b4b.png)


💡 19. Wyświetl imię i nazwisko aktora o id 4 i tytuł filmu, w którym zagrał.

```sql
SELECT a.actor_id, a.name, a.surname, m.title
FROM actors AS a
JOIN cast AS c
	ON a.actor_id = c.actor_id
JOIN movies AS m
	ON m.movie_id = c.movie_id
WHERE a.actor_id = 4;
```

![19](https://user-images.githubusercontent.com/49365894/205619366-444e0381-6913-4256-bab0-11640669c903.png)


💡 20. A gdzie nasza HONIA!? Dodaj do tabeli customers nową krotkę, gdzie customer_id = 7, name = Honia, surname = Stuczka-Kucharska, email = [honia@mail.com](mailto:honia@mail.com) oraz pseudonym = Hoa.

```sql
INSERT INTO customers (customer_id, name, surname, email, pseudonim)
VALUES 
	(7,'Honia', 'Stuczka-Kucharska', 'honia@mail.com', 'Hoa');
```

![20](https://user-images.githubusercontent.com/49365894/205619413-4d67cce2-54fe-4163-a864-42a7787d77af.png)

## Subtask 2
12/15 punktów :blush:

<p align="center">
  <img src="https://user-images.githubusercontent.com/49365894/205629021-6e665378-0df8-45a3-bbba-5085ffe597d5.png">
</p>

źródło: https://pixabay.com/ -|


