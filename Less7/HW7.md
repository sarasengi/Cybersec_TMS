# Домашняя работа №7

## Типы атак I, OWASP top 10
_CVE, CWE, CAPEC, Injection, SQL_

### 1. Изучить SQL запросы.
- Пройти как можно больше заданий в SQLBOLT

Пока остановилась на 7 лабе, и то она мне туго далась уже:<br>
![](pics/SQL.png)

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
