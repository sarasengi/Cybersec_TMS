# Урок №35  
### PENTEST  
Теория  


* [Лекция](35_Pentest.pdf)
* [Домашняя работа](HW35_36.md)


---

## Mini-quize по прошлым темам:

<details>
  <summary>1. Что такое OSINT?</summary>
<br>

**OSINT (Open Source Intelligence)** — это процесс сбора и анализа данных из открытых источников, таких как интернет, социальные сети, регистрационные базы данных, СМИ и многое другое.  

---

</details>

<details>
  <summary>2. Какие основные источники для OSINT?</summary>
<br>

Основные источники:  
- **Поисковые системы:** Google, Bing, Yandex.  
- **Социальные сети:** Facebook, Twitter, LinkedIn.  
- **Регистры доменных имен:** WHOIS, DNS-записи.  
- **Открытые базы данных:** Судебные реестры, государственные архивы.  
- **Облачные утечки:** Pastebin, Have I Been Pwned.  

---

</details>

<details>
  <summary>3. Для чего проводить разведку по открытым источникам в сфере кибербеза?</summary>
<br>

**Цели разведки OSINT в кибербезопасности:**  
- Выявление уязвимостей и утечек данных.  
- Анализ инфраструктуры компании для предотвращения атак.  
- Сбор информации для пентестов или расследований.  

---

</details>

<details>
  <summary>4. Что является основой для безопасного и эффективного OSINT?</summary>
<br>

Основы OSINT:  
- **Этичность:** Соблюдение законов и моральных норм.  
- **Легальность:** Использование только разрешённых инструментов и источников.  
- **Тщательность:** Проверка достоверности собранной информации.  
- **Анонимность:** Защита своей личности и методик сбора данных.  

---

</details>

<details>
  <summary>5. Какие могут быть негативные аспекты OSINT?</summary>
<br>

**Негативные аспекты OSINT:**  
- Использование собранных данных злоумышленниками.  
- Нарушение приватности объектов исследования.  
- Риск утечки информации об исследователе.  

---

</details>

<details>
  <summary>6. Какие принципы следует соблюдать при OSINT?</summary>
<br>

**Принципы OSINT:**  
- Законность и этичность.  
- Чёткое определение целей исследования.  
- Конфиденциальность полученных данных.  
- Использование проверенных инструментов.  

---

</details>

<details>
  <summary>7. Какую информацию мы можем разыскать при помощи OSINT?</summary>
<br>

С помощью OSINT можно найти:  
- Контактные данные (email, телефон).  
- Утечки паролей и аккаунтов.  
- Информацию о компании (сотрудники, инфраструктура).  
- Доменные записи, IP-адреса, поддомены.  

---

</details>

---

## Mini-quize по новой теме:

<details>
  <summary>1. Что такое «Пентест»? Как вы понимаете данное слово?</summary>
<br>

**Пентест (Penetration Testing)** — это метод проверки безопасности системы, сети или приложения, при котором моделируются действия злоумышленников для поиска уязвимостей.  

---

</details>

<details>
  <summary>2. Как подразделяется тестирование на проникновение?</summary>
<br>

Пентест подразделяется на:  
1. **Black-box:** Без предоставления информации о системе.  
2. **White-box:** С полным доступом к документации и исходному коду.  
3. **Gray-box:** Частичный доступ к информации.  

---

</details>

<details>
  <summary>3. Может ли при пентесте применяться OSINT?</summary>
<br>

Да, OSINT активно применяется на этапе разведки для сбора информации о цели:  
- Сбор данных о сотрудниках.  
- Анализ доменных записей, поддоменов.  
- Поиск утечек данных.  

---

</details>

<details>
  <summary>4. Из каких этапов должен состоять пентест?</summary>
<br>

Основные этапы пентеста:  
1. **Подготовка:** Согласование целей и объема работ.  
2. **Разведка:** Сбор информации о цели.  
3. **Сканирование:** Поиск уязвимостей с помощью автоматических инструментов.  
4. **Эксплуатация:** Проверка возможности эксплуатации найденных уязвимостей.  
5. **Отчёт:** Документирование результатов и рекомендаций.  

---

</details>

<details>
  <summary>5. Для чего применяется пентест?</summary>
<br>

**Цели пентеста:**  
- Выявление и устранение уязвимостей.  
- Проверка устойчивости систем к реальным атакам.  
- Улучшение уровня информационной безопасности.  

---

</details>

<details>
  <summary>6. Могут ли применяться автоматизированные средства при пентесте?</summary>
<br>

Да, автоматизированные инструменты упрощают и ускоряют процесс пентеста. Примеры:  
- **Nmap:** Сканирование сети.  
- **Burp Suite:** Тестирование веб-приложений.  
- **Metasploit:** Эксплуатация уязвимостей.  

---

</details>

<details>
  <summary>7. Какие основные тенденции в тестировании на проникновение?</summary>
<br>

**Основные тенденции:**  
- Использование автоматизации и ИИ.  
- Внедрение пентестов в процессы DevSecOps.  
- Адаптация к облачным и гибридным инфраструктурам.  
- Увеличение спроса на специализированные тесты (например, API, IoT).  

---

</details>

---

## План занятия:

<details>
  <summary>1. Рассмотрим что такое pentest, для чего он применяется</summary>
<br>

Разберём, что пентест — это имитация реальных атак с целью выявления уязвимостей.  
**Применение:**  
- Оценка защищённости.  
- Проверка соответствия стандартам (например, PCI DSS).  

---

</details>

<details>
  <summary>2. Рассмотрим как его проводят, где и зачем</summary>
<br>

**Проведение пентеста:**  
- На системах, сетях, приложениях.  
- В корпоративных и облачных средах.  
**Цель:**  
- Предотвращение утечек данных.  
- Повышение устойчивости к угрозам.  

---

</details>

<details>
  <summary>3. Основные направления в тестировании</summary>
<br>

Основные направления:  
- **Сети и инфраструктура:** Поиск уязвимостей в сетевых устройствах.  
- **Веб-приложения:** SQL-инъекции, XSS.  
- **API:** Проверка авторизации и безопасности данных.  
- **IoT:** Тестирование встроенных устройств.  

---

</details>

<details>
  <summary>4. Так же рассмотрим основные тенденции и познакомимся с инструментами</summary>
<br>

**Тенденции:**  
- Увеличение автоматизации.  
- Расширение тестов на облачные и контейнерные среды.  

**Инструменты:**  
- **Nmap:** Для сканирования сетей.  
- **Burp Suite:** Для анализа веб-приложений.  
- **Metasploit:** Для создания и эксплуатации эксплойтов.  

---
</details>
