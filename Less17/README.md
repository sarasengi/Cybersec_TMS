# Урок №17
## Защита инфраструктуры приложений

* [Лекция](17-Защита_инфраструктуры_приложений.pdf)
* [Домашняя работа](HW17.md)


## Mini-quize по прошлым темам:
<details>
  <summary>В какое место сетевой схемы устанавливают IDS/IPS?</summary>
<br>
IDS (система обнаружения вторжений) и IPS (система предотвращения вторжений) обычно устанавливают на границе между внутренней сетью и внешней, чтобы контролировать весь входящий и исходящий трафик.

Иногда IDS/IPS размещают в ключевых точках сети, например, рядом с критически важными серверами, чтобы защитить их от потенциальных угроз.

IDS часто ставят в режиме мониторинга, чтобы обнаруживать аномалии, а IPS — в активной защите, чтобы блокировать подозрительные действия в реальном времени.
 
---
  
</details>

<details>
  <summary>Что такое Windows Defender?</summary>
<br>
Windows Defender — это встроенная антивирусная программа для Windows, предназначенная для защиты системы от вирусов, шпионских программ, троянов и других угроз.

Она обеспечивает защиту в реальном времени и регулярно обновляет базы данных вредоносного ПО, чтобы быть в курсе новых угроз.

Помимо антивирусной защиты, Windows Defender также включает брандмауэр и инструменты для родительского контроля, что делает его основным защитником безопасности на устройствах Windows.
 
---
 
</details>


<details>
  <summary>Как можно защититься от DDoS?</summary>
<br>
Защита от DDoS-атак требует комбинированного подхода.

Один из методов — использование защитных инструментов, таких как брандмауэры и специальные сервисы от провайдеров (например, Cloudflare или Akamai), которые помогают фильтровать и распределять трафик.

Другой способ — настроить сеть так, чтобы обнаруживать аномальные пики трафика и быстро ограничивать его.

Можно также использовать распределение нагрузки (load balancing), чтобы снижать риск перегрузки одного сервера. 

Хорошей практикой будет использование резервных серверов и дополнительных каналов связи.

 
---
 
</details>


<details>
  <summary>Как можно защитить почтовый сервер?</summary>
<br>
Защита почтового сервера включает несколько аспектов.

Во-первых, стоит использовать фильтрацию спама и вредоносного ПО, чтобы предотвратить получение вредоносных писем.

Второе — это настройка DMARC, SPF и DKIM-записей, которые помогают удостовериться, что только разрешённые отправители могут отправлять письма от имени вашего домена.

Нужно также применять шифрование данных и протоколы безопасности, такие как TLS, чтобы обеспечить безопасную передачу писем.

И, конечно, регулярные обновления программного обеспечения почтового сервера и мониторинг активности помогут вовремя обнаружить и устранить угрозы.
 
---
 
</details>


<details>
  <summary>Что означает CVSS?</summary>
<br>
CVSS (Common Vulnerability Scoring System) — это общая система оценки уязвимостей, которая помогает определять, насколько серьёзна и опасна конкретная уязвимость.

Она оценивает несколько факторов, включая лёгкость эксплуатации, возможные последствия для конфиденциальности и целостности данных,

и даёт итоговую оценку (от 0 до 10 баллов), которая помогает понять приоритетность устранения угроз.

CVSS — стандарт, который широко используется для управления рисками в информационной безопасности.
 
---
 
</details>


<details>
  <summary>Что такое iptables и чем он может быть полезен?</summary>
<br>
Iptables — это утилита для настройки правил фильтрации трафика в Linux.

С её помощью можно определять, какие пакеты данных можно пропускать, а какие блокировать, основываясь на их адресах, портах и других параметрах.

Iptables полезен для настройки брандмауэра на уровне сети и позволяет администратору управлять доступом к сети, защищая серверы и данные от несанкционированных попыток доступа.

Это мощный инструмент для построения сетевой безопасности.
 
---
 
</details>


<details>
  <summary>Что такое Zero Trust?</summary>
<br>
Zero Trust — это модель безопасности, которая исходит из принципа "никому не доверять".

Она предполагает, что все пользователи, устройства и соединения, даже если они находятся внутри сети, должны проходить строгую проверку перед получением доступа к ресурсам.

Zero Trust требует аутентификации, авторизации и постоянного мониторинга активности, чтобы минимизировать риски от потенциальных внутренних и внешних угроз.
 
---
 
</details>



## Mini-quize по новой теме:

<details>
  <summary>Что такое виртуализация?</summary>
<br>
Виртуализация — это процесс создания виртуальной версии компьютерных ресурсов, таких как серверы, хранилища, операционные системы или сетевые устройства.

Виртуализация позволяет запускать несколько виртуальных машин (ВМ) на одном физическом устройстве. Это эффективно распределяет ресурсы, поскольку каждая ВМ работает независимо, используя ресурсы по необходимости. Например, вместо одного физического сервера можно создать несколько ВМ с разными ОС для тестирования приложений.

Примеры систем виртуализации — это **VMware**, **Hyper-V** и **KVM**.

---

</details>

<details>
  <summary>Что означает термин отказоустойчивый сервер?</summary>
<br>
Отказоустойчивый сервер — это сервер, спроектированный так, чтобы продолжать работу даже при возникновении аппаратных или программных сбоев. 

Чтобы достичь отказоустойчивости, серверы используют дублирование компонентов: например, несколько жёстких дисков (RAID), резервные источники питания и сетевые адаптеры. Такой сервер автоматически переключается на дублирующие компоненты в случае неисправности.

Например, в банковских системах и в медицинских учреждениях отказоустойчивость критична, так как перерывы в работе могут повлиять на важные операции.

---

</details>

<details>
  <summary>Как осуществляется безопасность облачных сред?</summary>
<br>
Безопасность облачных сред обеспечивается с помощью множества методов и инструментов.

Во-первых, это шифрование данных, как при передаче (например, через HTTPS), так и при хранении, чтобы предотвратить несанкционированный доступ. Во-вторых, используется контроль доступа — облачные провайдеры предоставляют инструменты для управления правами пользователей, например, **AWS Identity and Access Management (IAM)**. 

Также применяются сетевые защиты, такие как виртуальные брандмауэры и системы предотвращения вторжений (IPS). Например, **Microsoft Azure Security Center** помогает мониторить и управлять безопасностью облачной среды.

---

</details>

<details>
  <summary>Есть ли категорирование уязвимостей для Docker, как вы думаете, она называется?</summary>
<br>
Да, уязвимости для Docker и других контейнерных технологий классифицируются, и система называется **Docker Security Scanning**.

Docker использует систему оценки уязвимостей, которая классифицирует их по CVE (Common Vulnerabilities and Exposures) и применяет CVSS (Common Vulnerability Scoring System) для определения критичности уязвимостей. Docker также выпускает свои рекомендации для улучшения безопасности контейнеров, например, ограничение привилегий контейнеров и использование подписанных образов.

---

</details>

<details>
  <summary>Что такое Docker Compose, можно ли создать собственный?</summary>
<br>
Docker Compose — это инструмент для упрощённого управления многоконтейнерными приложениями. Он позволяет описать конфигурацию всех контейнеров приложения в одном YAML-файле (обычно `docker-compose.yml`). В этом файле можно задать все параметры контейнеров, включая сети, порты, переменные окружения и зависимые службы, чтобы затем запустить все контейнеры одной командой: `docker-compose up`.

Да, можно создать собственный файл Docker Compose. Например, для веб-приложения можно создать конфигурацию, которая описывает контейнеры для базы данных и самого веб-сервера.

---

</details>
