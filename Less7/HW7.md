# Домашняя работа №7

## Типы атак I, OWASP top 10
_CVE, CWE, CAPEC, Injection, SQL_

### 1. Изучить SQL запросы.
- Пройти как можно больше заданий в SQLBOLT

Пока остановилась на 7 лабе, и то она мне туго далась уже:<br>
![](pics/SQL.png)

<details><summary>Вопросы и ответы с заданий:</summary>
  
1:

Find the title of each film<br>
```SELECT title FROM movies;```

Find the director of each film<br>
```SELECT director FROM movies;```

Find the title and director of each film<br>
```SELECT director,title FROM movies;```

Find the title and year of each film<br>
```SELECT title,year FROM movies;```

Find all the information about each film<br>
```SELECT * FROM movies;```

2:

Find the movie with a row id of 6<br>
```SELECT * FROM movies where id=6;```

Find the movies released in the years between 2000 and 2010<br>
```SELECT * FROM movies where year between 2000 and 2010;```

Find the movies not released in the years between 2000 and 2010<br>
```SELECT * FROM movies where year not between 2000 and 2010;```

Find the first 5 Pixar movies and their release year<br>
```SELECT * FROM movies where id between 1 and 5;```

3:

Find all the Toy Story movies<br>
```SELECT * FROM movies where title like "Toy Story%";```

Find all the movies directed by John Lasseter<br>
```SELECT * FROM movies where director="John Lasseter";```

Find all the movies (and director) not directed by John Lasseter<br>
```SELECT * FROM movies where not director="John Lasseter";```

Find all the WALL-* movies<br>
```SELECT * FROM movies where title like "WALL-%";```

4:

List all directors of Pixar movies (alphabetically), without duplicates<br>
```SELECT DISTINCT director FROM movies order by director;```

List the last four Pixar movies released (ordered from most recent to least)<br>
```SELECT * FROM movies order by year desc limit 4;```

List the first five Pixar movies sorted alphabetically<br>
```SELECT * FROM movies order by title limit 5;```

List the next five Pixar movies sorted alphabetically<br>
```SELECT * FROM movies order by title limit 5 offset 5;```

5:

List all the Canadian cities and their populations<br>
```SELECT * FROM north_american_cities where country="Canada";```

Order all the cities in the United States by their latitude from north to south<br>
```SELECT city, latitude FROM north_american_cities where country="United States" order by latitude desc;```

List all the cities west of Chicago, ordered from west to east<br>
```SELECT * FROM north_american_cities where longitude < "-87.629798" order by longitude;```

List the two largest cities in Mexico (by population)<br>
```SELECT * FROM north_american_cities WHERE country="Mexico" order by population desc limit 2;```

List the third and fourth largest cities (by population) in the United States and their population<br>
```SELECT city, population FROM north_american_cities WHERE country="United States" order by population desc limit 2 offset 2;```

6:

Find the domestic and international sales for each movie<br>
```SELECT title, domestic_sales, international_sales from movies join boxoffice ON movies.id = boxoffice.movie_id;```

Show the sales numbers for each movie that did better internationally rather than domestically<br>
```SELECT title, domestic_sales, international_sales FROM movies JOIN boxoffice ON movies.id = boxoffice.movie_id where boxoffice.international_sales > boxoffice.domestic_sales;```

List all the movies by their ratings in descending order<br>
```SELECT title, rating FROM movies join boxoffice on movies.id = boxoffice.movie_id order by rating desc;```

7:

Find the list of all buildings that have employees<br>
```SELECT DISTINCT building FROM employees;```

Find the list of all buildings and their capacity<br>
```SELECT * FROM buildings;```

List all buildings and the distinct employee roles in each building (including empty buildings)<br>
```SELECT DISTINCT role, building_name from buildings left join employees ON building_name = building;```

</details>

### 2. Лабораторные работы по OWASP TOP 10.
- Выполнить 2 лабораторные работы из практики Brocken Access Control<br>
  - Lab Broken Access Controll 1<br>
![](pics/Burp_edit_cookie.png)<br>
![](pics/Admin_panel_enabled.png)<br>
![](pics/Solve_lab.png)<br>
  - Lab Broken Access Controll 2<br>
![](pics/access_labs_done.png)<br>
- Выполнить 1 лабораторную работу из практики Injections<br>
  - Lab Injection 1<br>
![](pics/SQL_inj_done.png)<br>
- Выполнить 1 лабораторную работу из практики Server-Side Request Forgery<br>
  - Lab SSRF 1<br>
 ![](pics/SSRF.png)<br>
 ![](pics/SSRF_lab_done.png)<br>

Вот что в итоге в учётке отображается
 ![](pics/academy.png)<br>


### 3.  Тренировка поиска уязвимостей на примере OWASP Juice Shop
 - OWASP Juice Shop

Docker поставила на машину с Kali, чтобы не плодить кучу VPS, вот есть [мануал](https://www.kali.org/docs/containers/installing-docker-on-kali/)<br>
 ![](pics/Docker_installed_kali.png)<br>
 Контейнер с Juice Shop запустила, но заданий выполнила мало<br>
 ![](pics/juicashop_dockerpull.png)<br>
 ![](pics/juicashop_dockerrunls.png)<br>
 ![](pics/Juiceshop_works.png)<br>
 ![](pics/scoreboard.png)<br>


### Ссылки на дополнительные ресурсы
[Тренировка написания SQL запросов в SQLBOLT](https://sqlbolt.com)<br>
[Lab Broken Access Controll 1](https://portswigger.net/web-security/access-control/lab-user-role-controlled-by-request-parameter)<br>
[Lab Broken Access Controll_2](https://portswigger.net/web-security/access-control/lab-user-role-controlled-by-request-parameter)<br>
[Lab Injection 1](https://portswigger.net/web-security/sql-injection/lab-retrieve-hidden-data)<br>
[Lab SSRF 1](https://portswigger.net/web-security/ssrf/lab-basic-ssrf-against-localhost)<br>
[OWASP Juice Shop](https://spy-soft.net/owasp-juice-shop/)<br>
[Juice Shop Docker](https://hub.docker.com/r/bkimminich/juice-shop)<br>
