# Урок №19
## Основные виды СЗИ

* [Лекция](19_szi.pdf)
* [Домашняя работа](HW19.md)


## Mini-quize по прошлым темам:

<details>
  <summary>Какие принципы работы WAF вы знаете?</summary>
<br>
WAF (Web Application Firewall) — это брандмауэр для веб-приложений, который защищает веб-сайты и приложения от специфических атак, таких как SQL-инъекции, межсайтовый скриптинг (XSS) и другие угрозы.

Основные принципы работы WAF:
- **Сигнатурный анализ:** WAF проверяет трафик на наличие известных шаблонов вредоносных запросов (сигнатур). Если запрос совпадает с шаблоном угрозы, он блокируется.
- **Поведенческий анализ:** WAF отслеживает аномалии в поведении трафика, например, резкое увеличение запросов с одного IP, что может указывать на атаку.
- **Фильтрация по правилам:** Администратор может вручную настроить правила, которые будут блокировать или разрешать определённые типы запросов.

WAF может быть размещён на уровне сети или на сервере, и он полезен для предотвращения распространённых атак на веб-приложения.

---

</details>

<details>
  <summary>Какие задачи можно решать с помощью скриптов автоматизации?</summary>
<br>
Скрипты автоматизации помогают выполнять рутинные и повторяющиеся задачи быстрее и эффективнее.

Скрипты можно использовать для:
- **Резервного копирования:** Создание копий данных по расписанию.
- **Мониторинга систем:** Автоматическое отслеживание ресурсов (памяти, дисков) и состояния системы.
- **Управления пользователями:** Создание учётных записей, обновление паролей и настройка прав доступа.
- **Управления сетью:** Конфигурирование сетевых параметров и проверка сетевого подключения.
- **Проверки безопасности:** Запуск сканеров уязвимостей, проверка логов на подозрительные действия.

Скрипты позволяют автоматизировать множество задач, которые обычно требуют много времени, что делает их незаменимыми в администрировании и ИТ-безопасности.

---

</details>

<details>
  <summary>Для чего предназначены команды ifconfig, netstat, tcpdump</summary>
<br>
Эти команды — полезные инструменты для сетевого администрирования в Linux.

- **ifconfig:** Отображает информацию о конфигурации сетевых интерфейсов (например, IP-адреса, маски подсетей). Её часто используют для настройки сетевых параметров.
- **netstat:** Показывает активные соединения, порты, маршруты и сетевую статистику. Полезна для мониторинга подключения и диагностики сетевых проблем.
- **tcpdump:** Перехватывает и анализирует сетевые пакеты. Её можно использовать для детального анализа сетевого трафика и выявления подозрительных пакетов.

Эти команды помогают отслеживать и управлять сетевыми соединениями, а также выявлять и устранять проблемы с сетью.

---

</details>

<details>
  <summary>Какой командой можно посмотреть список сервисов на Linux?</summary>
<br>
Список активных сервисов в Linux можно посмотреть командой:

```shell
systemctl list-units --type=service
```

Эта команда показывает активные сервисы и их статусы, что удобно для мониторинга работы системных служб.

Также, для более старых систем можно использовать команду:
```shell
service --status-all
```

Эта команда выводит список всех сервисов и их состояния.

---

</details>


## Mini-quize по новой теме:

<details>
  <summary>Какие отделы есть в SOC?</summary>
<br>
SOC (Security Operations Center) — это центр безопасности, который следит за защитой компании от киберугроз. 

Основные отделы SOC:
- **Аналитики безопасности (Security Analysts):** Первичная защита, мониторинг и расследование инцидентов.
- **Операторы (Security Engineers):** Настраивают системы безопасности, управляют инфраструктурой.
- **Группа реагирования на инциденты (Incident Response Team):** Отвечают за анализ и устранение угроз.
- **Команда управления уязвимостями (Vulnerability Management Team):** Проводят сканирование и исправление уязвимостей.
- **Разработчики и архитекторы безопасности:** Обеспечивают защиту на уровне архитектуры сети и приложений.

Эти отделы работают вместе, чтобы обнаруживать и предотвращать атаки.

---

</details>

<details>
  <summary>Для чего предназначено средство PAM?</summary>
<br>
PAM (Pluggable Authentication Modules) — это система модулей для настройки аутентификации в Linux.

PAM даёт гибкие возможности для управления доступом к системе, например:
- Требовать дополнительные проверки для входа в систему.
- Настроить двухфакторную аутентификацию.
- Ограничивать доступ по IP или времени суток.

С помощью PAM администраторы могут задавать строгие правила для безопасности и ограничивать доступ к системе.

---

</details>

<details>
  <summary>Что такое YARA?</summary>
<br>
YARA — это инструмент для обнаружения вредоносных программ на основе определённых правил.

С помощью YARA можно написать правила, которые описывают шаблоны вредоносного кода. YARA сканирует файлы и ищет совпадения по этим шаблонам, что позволяет находить вредоносное ПО по его характеристикам, а не только по конкретным сигнатурам.

YARA используется во многих антивирусах и системах кибербезопасности для детального анализа файлов.

---

</details>

<details>
  <summary>Для чего предназначена Data Leak Prevention?</summary>
<br>
Data Leak Prevention (DLP) — это технологии, которые помогают предотвращать утечки данных.

DLP мониторит и блокирует передачу конфиденциальной информации, такую как файлы с персональными данными или коммерческой тайной. Например, если сотрудник попытается отправить защищённый документ по электронной почте за пределы компании, DLP может заблокировать это действие и уведомить администратора.

Это важный инструмент для предотвращения несанкционированного обмена конфиденциальными данными.

---

</details>

<details>
  <summary>Для чего применяется NGFW и как она работает?</summary>
<br>
NGFW (Next-Generation Firewall) — это "брандмауэр нового поколения", который объединяет функции традиционного брандмауэра с возможностями для улучшенной безопасности.

В отличие от стандартных брандмауэров, NGFW может:
- Отслеживать трафик на уровне приложений (например, блокировать доступ к вредоносным сайтам).
- Распознавать и блокировать сложные угрозы, такие как эксплойты.
- Работать в связке с другими средствами безопасности, например, с системами предотвращения вторжений (IPS).

NGFW используется для более точного управления доступом и защиты от сложных атак.

---

</details>


## План занятия:

<details>
  <summary>Антивирусы, сигнатурный поиск</summary>
<br>
Антивирусы — это программы, которые обнаруживают и удаляют вредоносное ПО. Сигнатурный поиск — это один из методов обнаружения, при котором антивирус ищет в файлах известные сигнатуры (шаблоны) вредоносного кода.

Когда антивирус обнаруживает файл с известной сигнатурой вируса, он блокирует или удаляет его. Этот метод эффективен для обнаружения известных угроз, но может быть менее эффективен против новых или модифицированных вирусов.

---

</details>

<details>
  <summary>Firewall, Web Application Firewall и Next Generation Firewalls</summary>
<br>
Брандмауэры (Firewalls) — это системы, которые блокируют несанкционированный доступ к сети, защищая устройства и данные.

- **Firewall:** Фильтрует трафик на уровне сети.
- **WAF (Web Application Firewall):** Защищает веб-приложения от угроз, например, SQL-инъекций и XSS.
- **NGFW (Next Generation Firewall):** Более продвинутый брандмауэр, который может блокировать сложные атаки, отслеживать трафик приложений и работать с другими средствами безопасности.

Эти средства играют ключевую роль в сетевой защите и предотвращении угроз.

---

</details>

<details>
  <summary>Data Leak Prevention, защита от утечек и PAM</summary>
<br>
Data Leak Prevention (DLP) — это технология, предотвращающая утечки данных, которая мониторит и ограничивает передачу конфиденциальной информации.

PAM (Pluggable Authentication Modules) — это система аутентификации, позволяющая создавать правила для доступа в системе и добавлять дополнительные проверки для безопасности.

Оба этих средства помогают контролировать доступ к данным и защищать от случайных или намеренных утечек информации.

---

</details>

<details>
  <summary>Понятие Security Operation Center</summary>
<br>
Security Operation Center (SOC) — это команда экспертов по кибербезопасности, которая круглосуточно отслеживает и защищает сети и данные компании. 

SOC включает различные отделы: аналитики безопасности, инженеры, группа реагирования на инциденты, специалисты по управлению уязвимостями и архитекторы безопасности. Каждый отдел в SOC выполняет свои задачи, но все они работают вместе, чтобы своевременно обнаруживать и предотвращать киберугрозы.

---

</details>

<details>
  <summary>XDR, EDR, MDR - теория</summary>
<br>
XDR (Extended Detection and Response), EDR (Endpoint Detection and Response) и MDR (Managed Detection and Response) — это различные методы и системы для обнаружения угроз и реагирования на них.

- **EDR:** Сосредоточен на обнаружении угроз на конечных точках (например, компьютерах сотрудников) и анализе данных об атаках.
- **XDR:** Объединяет информацию из различных источников (конечные точки, сеть, почта) для более комплексного анализа.
- **MDR:** Включает управляемые услуги по обнаружению и реагированию, где сторонние специалисты помогают мониторить и реагировать на угрозы.

Эти технологии помогают компаниям лучше понимать и защищаться от угроз.

---

</details>
