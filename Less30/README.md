# Урок №30
### Web Application Security

* [Лекция](30_Web_App_Sec.pdf)
* [Домашняя работа](HW30.md)



---


## Mini-quize по новой теме:

<details>
  <summary>1. Для чего нужен WAF, какой у него принцип работы?</summary>
<br>

WAF (Web Application Firewall) — это средство защиты веб-приложений, которое фильтрует и анализирует входящий и исходящий HTTP/HTTPS трафик.  

**Принцип работы:**  
- Анализ запросов на основе правил (например, OWASP CRS).  
- Обнаружение и блокировка вредоносных запросов, таких как SQL-инъекции, XSS и др.  
- Использование технологий на основе сигнатур, поведения или машинного обучения.  

---

</details>

<details>
  <summary>2. С какой проблемой мы можем столкнуться при работе с WAF?</summary>
<br>

Основные проблемы при работе с WAF:  
- **Ложные срабатывания:** Блокировка легитимных запросов.  
- **Производительность:** Влияние на скорость обработки запросов.  
- **Сложность настройки:** Требуется ручная настройка правил для специфичных приложений.  
- **Обход WAF:** Некоторые атаки могут быть пропущены, если WAF неправильно настроен.  

---

</details>

<details>
  <summary>3. Есть ли отличия между IPS и WAF?</summary>
<br>

Да, отличия между IPS (Intrusion Prevention System) и WAF следующие:  

- **IPS**:  
  - Защищает сетевую инфраструктуру.  
  - Работает на уровне сетевых протоколов (L3/L4).  
  - Блокирует атаки, такие как DDoS, сканирование портов.  

- **WAF**:  
  - Защищает веб-приложения.  
  - Работает на уровне приложения (L7).  
  - Ориентирован на защиту от SQL-инъекций, XSS, и других атак.  

---

</details>

<details>
  <summary>4. Как вы думаете, чем платное решение WAF лучше Open source?</summary>
<br>

**Платные решения WAF** могут быть лучше за счёт:  
- Поддержки от вендора.  
- Обновлений правил в реальном времени.  
- Расширенной аналитики и интеграции с SIEM.  
- Высокой производительности и надёжности.  
- Удобного интерфейса для управления и настройки.  

**Open Source WAF** (например, ModSecurity) хороши для начального использования, но требуют больше ресурсов на настройку и поддержку.  

---

</details>

<details>
  <summary>5. В какое место сетевой схемы устанавливают WAF?</summary>
<br>

WAF устанавливают между пользователем и веб-сервером:  
- Перед веб-сервером, чтобы фильтровать входящий трафик.  
- Часто интегрируется в сетевые устройства, такие как шлюзы или балансировщики нагрузки.  
- Может быть развернут в облаке (Cloud WAF) для защиты облачных приложений.  

---

</details>

---

## План занятия:

<details>
  <summary>1. Почему Веб популярен</summary>
<br>

Обсудим причины популярности веб-технологий:  
- Доступность через браузер без установки дополнительного ПО.  
- Возможность работы на разных устройствах (кросс-платформенность).  
- Простота обновления и масштабируемость веб-приложений.  

---

</details>

<details>
  <summary>2. Как работает WAF</summary>
<br>

Разберём архитектуру и принципы работы WAF:  
- Основные методы защиты (сигнатуры, поведенческий анализ).  
- Варианты развёртывания (интеграция в сервер, облако, аппаратные решения).  

---

</details>

<details>
  <summary>3. Какие ресурсы имеются для анализа безопасности</summary>
<br>

Ознакомимся с инструментами и платформами:  
- OWASP ZAP, Burp Suite.  
- NVD, Vulners.  
- OpenCVE для мониторинга новых уязвимостей.  

---

</details>

<details>
  <summary>4. Рассмотрим работу с WAF</summary>
<br>

На практике:  
- Установим и настроим ModSecurity.  
- Проверим работу правил Core Rule Set (CRS).  
- Изучим примеры сработок и настройку исключений.  

---

</details>

<details>
  <summary>5. Ознакомимся со стандартом тестирования</summary>
<br>

Разберём стандарт OWASP ASVS для проверки безопасности приложений:  
- Уровни тестирования (Basic, Standard, Advanced).  
- Основные категории тестов: аутентификация, управление сессиями, безопасность API.  

---

</details>

<details>
  <summary>6. Рассмотрим Client-side security и что означает DNSSEC</summary>
<br>

**Client-side security:**  
- Меры защиты на стороне клиента (CSP, ограничение ввода данных).  

**DNSSEC (Domain Name System Security Extensions):**  
- Технология, обеспечивающая защиту от подмены DNS-записей.  
- Использует цифровую подпись для проверки подлинности записей.  

---

</details>

<details>
  <summary>7. Узнаем, что есть кроме OWASP Top 10</summary>
<br>

Обсудим дополнительные ресурсы:  
- OWASP API Security Top 10.  
- CWE/SANS Top 25 Most Dangerous Software Errors.  
- Рекомендации NIST по безопасности.  

---

</details>

<details>
  <summary>8. Как защитить API gateways</summary>
<br>

Разберём подходы к защите API-шлюзов:  
- Аутентификация и авторизация (OAuth, JWT).  
- Ограничение запросов (Rate Limiting).  
- Валидация входных данных и мониторинг активности.  

---

</details>

<details>
  <summary>9. Что такое Антибот система</summary>
<br>

Антибот система — это инструмент, предназначенный для обнаружения и блокировки автоматизированных запросов (ботов).  

**Основные функции:**  
- Распознавание аномальной активности.  
- Использование CAPTCHA или JavaScript-челленджей.  
- Защита от парсинга контента и DDoS-атак.  

---

</details>

