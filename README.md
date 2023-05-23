# Task 1


## Subtask 1

10 points


## Subtask 3

I've decided to take part in this project to test my knowledge and abilities in practice.

I would like to gain more experience in software testing and acquire more advanced skills. I need to increase my chances of getting a job in IT within the next year :)


## Subtask 4

#### PURPOSE AND FUNCTIONALITIES OF THE WEB APP

This app has been designed to store and explore data about football players concerning their ratings, positions, performance/skills etc.

I would distinguish browsing in database with players’ performance details as main functionality, including data for matches and reports.

On that basis, I would discriminate other sub-functionalities including adding and editing: players, matches and reports.

Other sub-functionalities unrelated to data editing would be:
- downloading, printing and filtering data;
- contact with development team;
- changing the language.

UI design is simple - I assume that this type of application doesn’t have to be eye-catching as it is used mostly for storing some data. It is clear and easy to navigate.

#### INCONVENIENCES & PROPOSED IMPROVEMENTS

- taking into consideration security issues, I would suggest implementing automatic logout for long-term inactivity;
- there are some typos, e.g. Aktywnosć, zaaktualizowany;
- there are some inconsistencies in language - e.g. Filter table in Polish mode shows labels both in Polish and English (Imię, Nazwisko, Age, Pozycja, Klub, Rate);
- errors should be more informative - e.g. there may be information about lack of @ in email address instead of a vague note 'Cannot add player';
- the tables may be more readable if contrast is used (e.g. zebra stripes effect);
- using *input* tags inside *form* tag (instead *div*) would make HTML structure more semantic;
- in Slow 3G mode it takes almost a minute (57.78 s) to render Players Table (it takes about 25 s in Fast 3G mode) - it may be uncomfortable to operate for users;
- comment concerning RWD issue: in mobile mode the tables with data for Matches and Reports are still presented horizontally - users are not accustomed to scrolling form left to right (it may be more convenient to present the table vertically as it takes place in case of Players table);
- database search may be more convenient if there is pagination with buttons to navigate to first and last pages with a table;
- I haven’t found info where data for Events list comes from - it is just visible in a table but there is no place to add or edit this information in Edit Match Player form;
- there are no general databases for Matches, Reports and Events - they are just listed as inactive boxes with numbers - I have expected them to be presented e.g. as a table with data, similar to the database with Players details; the only reports and matches statistics I found are these redirected from Last updated report and they concern only one player;
- there is no information about the position of newly added player (I couldn’t find it in the table without filters searching).

#### BUGS
- ADD REPORT button doesn’t show a form to complete - it redirects the user to Matches table;
- there is no possibility to reach the final page of Players table - at some point it is stopped and cut into first column;
- data in columns Matches and Reports is transformed into [object Object] instead of numbers;
- column age in csv file shows date of birth instead of actual player’s age.


NOTE: This evaluation if far from ideal, but I stick to opinion that done is better than perfect :)

# Task 2

https://drive.google.com/drive/folders/1V1zmB-7uxiH26sD-tOFZ2nk8kGnRGGl3?usp=sharing

# Task 3

## Subtask 1
https://drive.google.com/file/d/1jnKSCmqpjT3jG8YSs30LsGL76evfmZIp/view?usp=sharing

## Subtask 2
https://drive.google.com/file/d/1sr_-x1v63rcBeAkcHzcpShTdVInNuJfJ/view?usp=sharing (part 1)

https://drive.google.com/file/d/1rMmH-oesHUfu6T7m2keCCnsLbu63Dnfy/view?usp=sharing (part 2)

## Subtask 3
https://drive.google.com/file/d/1JGQYzyYKcsz4h45WyoFbUNWXeXC64_IN/view?usp=share_link

# Task 4

## Subtask 1
https://drive.google.com/file/d/1M2igLOxoTvk_dpXol_pLWAbNWbFgeHgD/view?usp=share_link

## Subtask 3
https://drive.google.com/file/d/1PXRhk44QJy9tio9riqxbAZX8vdZ7dF6r/view?usp=share_link

# Task 5

## Subtask 1
SQL statements and operators: SELECT, SELECT DISTINCT, WHERE, AND/OR/NOT, ORDER BY, INSERT INTO, UPDATE, DELETE, LIKE, IN, BETWEEN, HAVING, EXISTS

## Subtask 3
#### 1. Wyświetl tabelę actors w kolejności alfabetycznej sortując po kolumnie surname.
SELECT * FROM actors ORDER BY surname;

<img width="250" alt="Zrzut ekranu 2023-05-23 o 12 43 29" src="https://github.com/substantia-innominata/software-testing-portfolio/assets/51747632/870944be-9496-451a-86de-787b7e959d4c">

#### 2. Wyświetl film, który powstał w 2019 roku.
SELECT * FROM movies WHERE year_of_production = 2019;

<img width="318" alt="Zrzut ekranu 2023-05-23 o 12 43 55" src="https://github.com/substantia-innominata/software-testing-portfolio/assets/51747632/fe9cd15e-55bc-423e-87f1-cb36c6758b05">

#### 3. Wyświetl wszystkie filmy, które powstały między 1900, a 1999 rokiem.
SELECT * FROM movies WHERE year_of_production BETWEEN 1900 AND 1999;

<img width="493" alt="Zrzut ekranu 2023-05-23 o 12 44 20" src="https://github.com/substantia-innominata/software-testing-portfolio/assets/51747632/576c1620-3a55-4c0e-8039-952f3a3ce691">

#### 4. Wyświetl JEDYNIE tytuł i cenę filmów, które kosztują poniżej 7$.S
SELECT DISTINCT title, price FROM movies WHERE price < 7;

<img width="290" alt="Zrzut ekranu 2023-05-23 o 12 44 49" src="https://github.com/substantia-innominata/software-testing-portfolio/assets/51747632/ab112b4a-93d4-4c29-9c6a-5654809f0ec1">

#### 6. Wyświetl klientów o id 2,4,6 wykorzystaj do tego warunek logiczny.
SELECT * FROM customers WHERE customer_id = 2 OR customer_id = 4 OR customer_id = 6

<img width="350" alt="Zrzut ekranu 2023-05-23 o 12 45 26" src="https://github.com/substantia-innominata/software-testing-portfolio/assets/51747632/34651fde-b49a-4d81-8a02-b591adb823c3">

#### 7. Wyświetl klientów o id 1,3,5 wykorzystaj do tego operator IN.
SELECT * FROM customers WHERE customer_id IN (1, 3, 5);

<img width="335" alt="Zrzut ekranu 2023-05-23 o 12 46 03" src="https://github.com/substantia-innominata/software-testing-portfolio/assets/51747632/406484c3-1de8-4bee-843f-060c597bc6e9">

#### 8. Wyświetl dane wszystkich osób z tabeli ‘actors’, których imię zaczyna się od ciągu “An”.
SELECT * FROM actors WHERE name LIKE 'An%';

<img width="215" alt="Zrzut ekranu 2023-05-23 o 12 46 33" src="https://github.com/substantia-innominata/software-testing-portfolio/assets/51747632/94e177dd-783c-4224-bdac-e60637fa5fab">

#### 9. Wyświetl dane klienta, który nie ma podanego adresu email.
SELECT * FROM customers WHERE email IS NULL;

<img width="292" alt="Zrzut ekranu 2023-05-23 o 12 46 55" src="https://github.com/substantia-innominata/software-testing-portfolio/assets/51747632/3e1ce8be-81f1-429d-908e-e8c541a72b63">

#### 10. Wyświetl wszystkie filmy, których cena wynosi powyżej 9$ oraz ich ID mieści się pomiędzy 2 i 8 movie_id.
SELECT * FROM movies WHERE price > 9 AND movie_id BETWEEN 2 AND 8;

<img width="359" alt="Zrzut ekranu 2023-05-23 o 12 47 27" src="https://github.com/substantia-innominata/software-testing-portfolio/assets/51747632/794ad747-6512-4081-8fcf-13f86f95d439">











