# Урок №34  
### OSINT (Open Source Intelligence)

* [Лекция](34_OSINT.pdf)
* [Домашняя работа](HW34.md)


---

## Mini-quize по прошлым темам:

<details>
  <summary>1. Что такое дамп памяти?</summary>
<br>

**Дамп памяти** — это копия содержимого оперативной памяти компьютера, сохраненная в файл для анализа.  

**Применение:**  
- Анализ работы приложений.  
- Поиск вредоносного кода.  
- Восстановление данных после сбоев.  

---

</details>

<details>
  <summary>2. Какие основные модули мы можем применять в Volatility?</summary>
<br>

Volatility — это мощный инструмент для анализа дампов памяти. Основные модули:  
- **pslist / psscan:** Выводит список процессов.  
- **dlllist:** Отображает загруженные DLL.  
- **filescan:** Ищет открытые файлы в памяти.  
- **netscan:** Анализ сетевых соединений.  
- **malfind:** Ищет потенциально вредоносные процессы.  

---

</details>

<details>
  <summary>3. Как мы можем обнаружить инцидент? Какой инструментарий поможет в этом?</summary>
<br>

**Обнаружение инцидента:**  
- Анализ логов систем и сетевых устройств (SIEM).  
- Мониторинг сетевого трафика (IDS/IPS).  
- Анализ поведения пользователей (UEBA).  

**Инструменты:**  
- SIEM-системы (Splunk, QRadar).  
- Антивирусы и EDR (Endpoint Detection & Response).  
- Песочницы для анализа файлов (Cuckoo Sandbox).  

---

</details>

<details>
  <summary>4. Из чего формируется ущерб от компьютерного инцидента?</summary>
<br>

**Ущерб от компьютерного инцидента** формируется из:  
1. **Финансовых потерь:** Утечка данных, штрафы, потеря клиентов.  
2. **Репутационных потерь:** Утрата доверия.  
3. **Операционных потерь:** Простой систем, снижение производительности.  
4. **Юридических последствий:** Судебные разбирательства, нарушение законов.  

---

</details>

---

## Mini-quize по новой теме:

<details>
  <summary>1. Какие основные «открытые» источники для OSINT?</summary>
<br>

Основные открытые источники:  
1. **Социальные сети:** Facebook, LinkedIn, Twitter.  
2. **Поисковые системы:** Google, Bing, Yandex.  
3. **Регистры доменных имен:** WHOIS, DNS.  
4. **Государственные базы данных:** Регистр предприятий, судебные архивы.  
5. **Облако утечек данных:** Pastebin, baza данных, Telegram-каналы.  

---

</details>

<details>
  <summary>2. Является ли противозаконным «пробив» по открытым источникам? Если использовать сливы баз данных?</summary>
<br>

**Законность зависит от страны и целей использования:**  
- Анализ открытых данных (например, WHOIS, соцсети) не нарушает закон, если информация находится в общем доступе.  
- Использование данных из утечек (например, сливов баз данных) может нарушать законы о конфиденциальности и авторских правах.  

**Совет:** Работайте только с легальными источниками и избегайте использования утечек.  

---

</details>

<details>
  <summary>3. Какие основные законы и моральные нормы необходимо соблюдать при проведении OSINT?</summary>
<br>

Основные правила:  
1. **Законы:**  
   - Закон о защите персональных данных (GDPR, 152-ФЗ в РФ).  
   - Законы о приватности и конфиденциальности.  

2. **Моральные нормы:**  
   - Уважение к частной жизни.  
   - Отказ от действий, которые могут навредить другим людям или организациям.  

3. **Принципы прозрачности:**  
   - Использовать OSINT исключительно в рамках согласованных целей (например, пентесты).  

---

</details>

<details>
  <summary>4. Для чего можно или нужно проводить OSINT?</summary>
<br>

OSINT используется для:  
1. **Кибербезопасности:**  
   - Поиск уязвимостей в инфраструктуре компании.  
   - Анализ утечек данных.  

2. **Юридических целей:**  
   - Проверка информации о компаниях или людях.  

3. **Разведки:**  
   - Сбор данных о конкурентах или угрозах.  

4. **Профилактики атак:**  
   - Идентификация фишинговых доменов, подозрительных IP.  

---

</details>

---

## План занятия:

<details>
  <summary>1. Рассмотрим основные открытые источники для сбора информации</summary>
<br>

Разберём, как использовать:  
- **Поисковые системы:** Углубленные операторы Google (например, `site:`, `filetype:`).  
- **Социальные сети:** Как находить скрытые профили или записи.  
- **Реестры:** Поиск через WHOIS, открытые госархивы.  

---

</details>

<details>
  <summary>2. Рассмотрим некоторые фишки для поиска информации</summary>
<br>

Практические приёмы:  
- Использование Google Dorking для точного поиска.  
- Настройка alert-систем (например, Google Alerts).  
- Автоматизация поиска с помощью инструментов (Recon-ng, SpiderFoot).  

---

</details>

<details>
  <summary>3. Попробуем некоторые инструменты и рассмотрим возможные пути для поиска информации</summary>
<br>

Протестируем инструменты:  
- **Recon-ng:** Модульная платформа для OSINT.  
- **Maltego:** Визуализация связей между данными.  
- **Shodan:** Поиск уязвимых устройств в интернете.  

*Задачи:*  
- Найти IP-адреса сервера компании.  
- Проанализировать DNS-записи через Recon-ng.  
- Создать граф связей в Maltego.  

---
</details>
