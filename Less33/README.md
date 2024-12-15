# Урок №33  
### Reverse Engineering  

* [Лекция](33_Reverse_engin.pdf)
* [Домашняя работа](HW33.md)


---

## Mini-quize по прошлым темам:

<details>
  <summary>1. Какие существуют политики резервного копирования?</summary>
<br>

Политики резервного копирования определяют подходы и правила сохранения данных для их восстановления в случае потери. Основные политики:  

1. **Полное резервное копирование:**  
   - Создается копия всех данных за один раз.  
   - **Достоинства:**  
     - Легко восстановить все данные из одной копии.  
     - Простота управления.  
   - **Недостатки:**  
     - Требует много времени и места для хранения.  
     - Высокая нагрузка на систему.  

2. **Дифференциальное резервное копирование:**  
   - Сохраняет изменения, произошедшие с последнего полного копирования.  
   - **Достоинства:**  
     - Быстрое создание копий.  
     - Восстановление быстрее, чем при инкрементальном копировании.  
   - **Недостатки:**  
     - Требует больше места, чем инкрементальное копирование.  

3. **Инкрементальное резервное копирование:**  
   - Сохраняет только изменения, произошедшие с момента последнего копирования (любого типа).  
   - **Достоинства:**  
     - Быстрое копирование и минимальное использование места.  
   - **Недостатки:**  
     - Восстановление данных требует последовательного применения всех копий.  

4. **Гибридное копирование:**  
   - Комбинация различных методов, часто используется в корпоративных системах для оптимизации затрат и времени.  

---

</details>

<details>
  <summary>2. В чем заключаются достоинства и недостатки групп в политиках администрирования AD?</summary>
<br>

**Достоинства групп в AD:**  
- **Централизованное управление:** Можно назначить права сразу нескольким пользователям, объединив их в группу.  
- **Простота настройки:** Группы упрощают управление доступом и политиками.  
- **Безопасность:** Использование групп минимизирует ошибки при ручном назначении прав.  
- **Масштабируемость:** Легко добавлять или удалять пользователей из групп, не изменяя настройки.  

**Недостатки:**  
- **Сложность мониторинга:** Большое количество групп и пересекающихся прав затрудняют контроль.  
- **Наследование ошибок:** Если группе назначены неправильные права, это может повлиять на всех её участников.  
- **Избыточность:** Часто создаются дублирующие группы, что увеличивает сложность управления.  

---

</details>

<details>
  <summary>3. Как работает механизм доменных имен AD, в целом?</summary>
<br>

Active Directory (AD) использует DNS (Domain Name System) для управления доменными именами и взаимодействия в сети.  

**Принципы работы:**  
1. **Иерархическая структура доменов:** AD организует ресурсы в деревья и леса, где каждый домен имеет уникальное имя.  
   *Пример:* `company.local`.  

2. **Роль контроллера домена (Domain Controller, DC):**  
   - Управляет пользователями, группами и компьютерами в домене.  
   - Использует DNS для локализации ресурсов и маршрутизации запросов.  

3. **Распределенные службы:**  
   - AD реплицирует данные между контроллерами домена.  
   - DNS помогает направлять запросы к нужному контроллеру.  

4. **Записи DNS:**  
   - `SRV` записи указывают на контроллеры домена и их службы (например, Kerberos или LDAP).  

---

</details>

<details>
  <summary>4. Если в компании развернуты только ОС Linux, какую AD вы бы использовали?</summary>
<br>

Для среды с Linux-серверами подойдут альтернативы Active Directory, например:  
- **FreeIPA:** Интеграция с Linux/UNIX. Поддерживает Kerberos, LDAP и DNS.  
- **Samba:** Реализует совместимость с протоколами Windows AD.  
- **OpenLDAP:** Универсальное решение для управления пользователями и группами.  
- **JumpCloud:** Облачное решение для управления идентификацией.  

Выбор зависит от потребностей: FreeIPA подходит для больших сетей, а Samba — для совместимости с Windows.  

---

</details>

---

## Mini-quize по новой теме:

<details>
  <summary>1. В чем разница между интерпретатором и компилятором?</summary>
<br>

**Интерпретатор:**  
- Выполняет код построчно, переводя команды программы в машинный язык в реальном времени.  
- **Достоинства:**  
  - Не требует предварительной компиляции.  
  - Удобен для отладки.  
- **Недостатки:**  
  - Медленнее компилятора, так как перевод происходит во время выполнения.  

**Компилятор:**  
- Преобразует весь исходный код в исполняемый файл до выполнения программы.  
- **Достоинства:**  
  - Высокая скорость выполнения программы.  
  - Исполняемые файлы не зависят от исходного кода.  
- **Недостатки:**  
  - Ошибки выявляются только на этапе компиляции.  

---

</details>

<details>
  <summary>2. C# с фреймворком .NET является компилируемым или интерпретируемым ЯП?</summary>
<br>

C# — компилируемый язык, но с особенностями:  
- Код компилируется в промежуточный язык (Intermediate Language, IL).  
- IL исполняется с помощью **CLR (Common Language Runtime)**, что добавляет черты интерпретатора.  

---

</details>

<details>
  <summary>3. Какие программы для написания кода вы знаете?</summary>
<br>

Популярные программы для написания кода:  
- **IDE:**  
  - Visual Studio, IntelliJ IDEA, PyCharm, Eclipse.  
- **Редакторы:**  
  - Visual Studio Code, Sublime Text, Atom.  
- **Консольные инструменты:**  
  - Vim, Nano.  

Каждый инструмент выбирается в зависимости от языка программирования и требований проекта.  

---

</details>

---

## План занятия:

<details>
  <summary>1. Разберемся как работают компиляторы</summary>
<br>

**Компиляторы**:  
- Переводят исходный код на высокоуровневом языке в машинный код.  
- Этапы работы:  
  1. **Лексический анализ:** Проверка синтаксиса и генерация токенов.  
  2. **Синтаксический анализ:** Построение дерева синтаксиса.  
  3. **Генерация кода:** Создание объектного файла или исполняемого файла.  

---

</details>

<details>
  <summary>2. Изучим основные опкоды и команды процессора</summary>
<br>

**Опкоды** — это машинные инструкции процессора.  
Примеры:  
- `MOV` — перемещение данных между регистрами.  
- `ADD/SUB` — арифметические операции.  
- `CMP` — сравнение данных.  
- `JMP` — переход к другой инструкции.  

*Важно:* Опкоды различаются между архитектурами (x86, ARM, RISC-V).  

---

</details>

<details>
  <summary>3. Подробнее изучим механизм подключения зависимостей PE файлов</summary>
<br>

**PE (Portable Executable) файлы:**  
- Формат исполняемых файлов Windows.  

**Зависимости:**  
- Подключаются через импортируемые библиотеки (DLL).  
- Таблица импорта хранит адреса используемых функций.  

Пример:  
- Программа подключает `kernel32.dll` для работы с файловой системой.  

---

</details>

<details>
  <summary>4. Рассмотрим отличия в архитектуре x86 и ia64</summary>
<br>

**x86:**  
- 32-битная архитектура.  
- CISC (Complex Instruction Set Computing): сложные инструкции.  
- Подходит для ПК и серверов.  

**IA-64:**  
- 64-битная архитектура.  
- Использует EPIC (Explicitly Parallel Instruction Computing).  
- Ориентирована на высокопроизводительные серверы.  

*Отличие:* IA-64 несовместима с x86, что усложняет перенос ПО.  

---

</details>
