# Урок №29
## Кодинг и уязвимости. Часть 2


* [Лекция](29_Coding_part_2.pdf)
* [Домашняя работа](HW29.md)


## Mini-quize по прошлым темам:

<details>
  <summary>Что такое КВОИ?</summary>
<br>

КВОИ (Ключевые показатели оценки инцидентов) — это метрики, которые используются для анализа и оценки событий информационной безопасности. Эти показатели помогают понять, насколько эффективно работает команда реагирования и как быстро устраняются угрозы.  

*Почему это важно:* КВОИ позволяют установить приоритеты для инцидентов, определить наиболее уязвимые зоны и убедиться, что ресурсы используются эффективно.  

*Пример КВОИ:*  
- Время обнаружения инцидента (Time to Detect).  
- Время реагирования на инцидент (Time to Respond).  
- Количество инцидентов, устранённых в рамках SLA (Service Level Agreement).  

---

</details>

<details>
  <summary>Какие основные документы регламентируют деятельность отделов / ЦК?</summary>
<br>

Основные документы, которые регулируют деятельность отделов или Центров кибербезопасности (ЦК), включают:  

1. **Политики информационной безопасности**: Устанавливают общие правила и требования по защите данных в организации.  
   *Пример:* Политика использования паролей.  

2. **Инструкции по реагированию на инциденты**: Подробно описывают шаги, которые должны быть предприняты при обнаружении угроз.  
   *Пример:* Порядок блокировки вредоносного трафика.  

3. **Стандарты и регламенты**: Международные (например, ISO/IEC 27001) или национальные стандарты (ГОСТ, НПА).  

4. **Отчётность и аудит**: Документы, фиксирующие инциденты, время реакции, результаты проверок.  

*Интересный факт:* Эти документы не только защищают, но и упрощают взаимодействие между отделами и внешними проверяющими.  

---

</details>

<details>
  <summary>Какие IOC первостепенны к сбору?</summary>
<br>

IOC (Indicators of Compromise, индикаторы компрометации) — это данные, которые помогают определить факт или попытку взлома.  

**Первостепенные IOC для сбора включают:**  
1. **IP-адреса**: Подозрительные IP, участвовавшие в атаках или сканировании.  
2. **Хэши файлов**: Уникальные идентификаторы вредоносных программ.  
3. **Доменные имена**: Адреса, с которых может осуществляться командное управление (C2-серверы).  
4. **URL-адреса**: Ссылки, ведущие к вредоносным файлам или фишинговым сайтам.  
5. **Артефакты системных логов**: Странные события, такие как многократные неудачные попытки входа или изменения конфигураций.  

*Пример:* Хэш известного трояна `e99a18c428cb38d5f260853678922e03`.  

---

</details>

<details>
  <summary>Для чего проводится аттестация ЦОК/ЦК?</summary>
<br>

Аттестация Центра обработки данных (ЦОК) или Центра кибербезопасности (ЦК) проводится для:  

1. **Проверки соответствия стандартам**: Убедиться, что центр соответствует установленным нормам и требованиям (например, ISO 27001 или требованиям регулятора).  

2. **Оценки уровня защищённости**: Проанализировать, насколько эффективно применены защитные меры.  

3. **Установления уровня зрелости**: Определить, насколько качественно и оперативно ЦК/ЦОК выполняет свои задачи.  

4. **Устранения уязвимостей**: В процессе аттестации выявляются слабые места и даются рекомендации по их устранению.  

*Пример выгоды:* Аттестация помогает предотвратить штрафы со стороны регуляторов и повысить доверие клиентов к уровню защищённости данных.  

---

</details>

## Mini-quize по новой теме:

<details>
  <summary>Какие математические операции в программировании вы знаете?</summary>
<br>

В программировании используются различные математические операции, которые можно разделить на несколько групп:

1. **Арифметические операции**:  
   - **Сложение (+)**: `a + b`, например, `2 + 3 = 5`.  
   - **Вычитание (-)**: `a - b`, например, `5 - 2 = 3`.  
   - **Умножение (*)**: `a * b`, например, `4 * 3 = 12`.  
   - **Деление (/)**: `a / b`, например, `10 / 2 = 5`.  
   - **Целочисленное деление (//)**: Деление с отбрасыванием дробной части, например, `10 // 3 = 3`.  
   - **Остаток от деления (%)**: `a % b`, например, `10 % 3 = 1`.  
   - **Возведение в степень (**)**: `a ** b`, например, `2 ** 3 = 8`.  

2. **Операции сравнения**:  
   - Больше (`>`), меньше (`<`), равно (`==`), больше или равно (`>=`), меньше или равно (`<=`), не равно (`!=`).  

3. **Операции сдвига**:  
   - Логический сдвиг влево (`<<`) и вправо (`>>`) для работы с битами.  

4. **Тригонометрические функции** (например, `sin`, `cos`, `tan`) и логарифмы.  
   *Пример:* Вычисление угла в треугольнике через `math.atan2`.  

*Применение:* Математические операции используются повсеместно: от подсчёта итоговой стоимости покупок до сложных вычислений в графике или криптографии.  

---

</details>

<details>
  <summary>Какие регулярные выражения вы знаете?</summary>
<br>

Регулярные выражения (регэкспы, RegEx) — это мощный инструмент для поиска, обработки и проверки текстовых данных. Примеры часто используемых регулярных выражений:  

1. **Символьные классы:**  
   - `\d` — любая цифра.  
   - `\w` — любой буквенно-цифровой символ.  
   - `\s` — пробел.  
   - `.` — любой символ.  

2. **Квантификаторы:**  
   - `*` — 0 или более повторений.  
   - `+` — 1 или более повторений.  
   - `?` — 0 или 1 повторение.  
   - `{n}` — ровно n повторений.  

3. **Якоря:**  
   - `^` — начало строки.  
   - `$` — конец строки.  

4. **Группировка и альтернативы:**  
   - `(abc)` — группа символов.  
   - `|` — "или". Например, `cat|dog` ищет "cat" или "dog".  

*Пример:* Проверка электронной почты:  
   `^[\w._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$`  

*Применение:* Регулярные выражения позволяют быстро находить и обрабатывать нужные данные в текстах, например, фильтровать лог-файлы или валидировать ввод пользователей.  

---

</details>

<details>
  <summary>К чему может привести отсутствие обработчиков ошибок и инструментов проверки кода?</summary>
<br>

Отсутствие обработчиков ошибок и инструментов проверки кода может привести к следующим последствиям:  

1. **Сбои в работе программ:** Без обработки ошибок программа может аварийно завершаться при любой нештатной ситуации.  
   *Пример:* Программа, делящая числа, завершится ошибкой при попытке деления на ноль.  

2. **Уязвимости в безопасности:** Некорректно обработанные исключения могут раскрыть информацию об архитектуре приложения злоумышленникам.  
   *Пример:* Публикация стека вызовов при ошибке подключения к базе данных.  

3. **Сложности в отладке и развитии проекта:** Наличие скрытых ошибок, которые могли быть устранены при проверке кода, замедлит разработку.  

4. **Непредсказуемое поведение:** Без инструментов проверки легко допустить ошибки, такие как утечка памяти, доступ к несуществующим данным или неправильная логика.  

*Решения:*  
- Использовать блоки `try-catch` для обработки ошибок.  
- Внедрять статические анализаторы кода (например, SonarQube).  
- Тестировать программы в разных сценариях, включая крайние случаи.  

---

</details>

<details>
  <summary>В чем заключается основная проблема при отсутствии валидации введенных данных?</summary>
<br>

Отсутствие валидации введённых данных — одна из главных причин уязвимостей в программном обеспечении. Проблемы включают:  

1. **Атаки злоумышленников:** Данные без проверки могут использоваться для выполнения вредоносного кода.  
   *Пример:* SQL-инъекция, когда ввод пользователя напрямую включается в SQL-запрос:  

```
SELECT * FROM users WHERE username = 'admin' OR '1'='1';
```


2. **Ошибки в работе программы:** Непредусмотренные форматы данных могут вызвать сбой или неожиданное поведение.  
*Пример:* Попытка сложить строку с числом, если ожидался только числовой ввод.  

3. **Снижение качества данных:** Невалидные данные могут испортить результаты анализа или работу системы.  

*Решения:*  
- Проверять длину, формат и тип введённых данных.  
- Использовать библиотеки валидации (например, Joi для JavaScript).  
- Применять регулярные выражения для проверки соответствия шаблону.  

---

</details>


## План занятия

<details>
  <summary>1. Математические операции и операторы сравнения на примере Python</summary>
<br>

В этом разделе разберём основные математические операции и операторы сравнения, которые используются в Python для работы с числами и другими типами данных.  

**Основные математические операции:**  
- Сложение (`+`), вычитание (`-`), умножение (`*`), деление (`/`).  
- Целочисленное деление (`//`): Отбрасывает дробную часть, например, `7 // 2 = 3`.  
- Остаток от деления (`%`): Результат — остаток, например, `7 % 2 = 1`.  
- Возведение в степень (`**`): Например, `2 ** 3 = 8`.  

**Операторы сравнения:**  
- `>` (больше), `<` (меньше), `>=` (больше или равно), `<=` (меньше или равно).  
- `==` (равно), `!=` (не равно).  

*Пример кода:*  

```
a = 5  
b = 3  
print(a + b)  # Сложение  
print(a > b)  # Сравнение: True  
```

*Применение:* Математические операции используются для расчётов, а операторы сравнения — в логике и проверках.  

---

</details>

<details>
  <summary>2. Регулярные выражения</summary>
<br>

Регулярные выражения (RegEx) позволяют находить, заменять и проверять текст на соответствие шаблонам.  

**Ключевые возможности:**  
- Поиск: Найти в тексте последовательности, соответствующие шаблону.  
- Замена: Заменить найденные шаблоны на заданные значения.  
- Валидация: Проверить, соответствует ли ввод определённым требованиям.  

**Пример регулярного выражения:**  
- Поиск email-адресов:  
  Шаблон: `^[\w._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$`.  

*Пример кода:*  

```
import re  

text = "Пример: test@example.com"  
match = re.search(r"[\w._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}", text)  
print(match.group() if match else "Email не найден")  
```

*Применение:* Используются для анализа логов, проверки ввода и парсинга текста.  

---

</details>

<details>
  <summary>3. Отсутствие шифрования и использование слабых алгоритмов шифрования</summary>
<br>

Отсутствие шифрования или использование слабых алгоритмов может привести к утечке данных, компрометации системы и увеличению риска атак.  

**Проблемы отсутствия шифрования:**  
- Конфиденциальные данные передаются в открытом виде (например, пароли, номера карт).  
- Любой, кто перехватит данные, сможет их прочитать.  

**Слабые алгоритмы шифрования:**  
- **MD5**: Подвержен коллизиям и не используется для безопасности.  
- **DES**: Устарел из-за низкой длины ключа (56 бит).  

**Решения:**  
- Использовать современные алгоритмы, такие как AES-256.  
- Применять SSL/TLS для передачи данных.  

*Пример:* Шифрование строки с использованием AES.  

---

</details>

<details>
  <summary>4. Ключ шифрования или пароли в исходном коде</summary>
<br>

Оставление ключей шифрования или паролей в исходном коде — грубая ошибка безопасности, которая может привести к:  
- Утечке конфиденциальных данных при доступе злоумышленников к исходному коду.  
- Лёгкой компрометации системы через просмотр репозиториев (например, GitHub).  

**Правильные подходы:**  
1. Хранить ключи и пароли в защищённых хранилищах (например, HashiCorp Vault, AWS Secrets Manager).  
2. Использовать переменные окружения для передачи конфиденциальных данных.  

*Пример:* Вместо жёсткого кода в программе:  

```
API_KEY = "секретный-ключ"  
```

Используйте переменные окружения:  

```
import os  
API_KEY = os.getenv("API_KEY")  
```

---

</details>

<details>
  <summary>5. Слабые и сильные алгоритмы хеширования</summary>
<br>

Хеширование используется для преобразования данных в уникальные строки фиксированной длины, которые сложно обратить назад.  

**Слабые алгоритмы:**  
- **MD5**: Лёгкость генерации коллизий делает его небезопасным.  
- **SHA-1**: Устаревший, подвержен атакам.  

**Сильные алгоритмы:**  
- **SHA-256**: Устойчив к коллизиям, используется для шифрования и проверки данных.  
- **bcrypt**: Алгоритм, специально разработанный для безопасного хеширования паролей, с настройкой сложности.  

*Пример использования bcrypt для хеширования паролей:*  

```
from bcrypt import hashpw, gensalt  

password = b"supersecret"  
hashed = hashpw(password, gensalt())  
print(hashed)  
```

*Совет:* Для хеширования паролей избегайте прямого использования SHA-256, вместо этого применяйте адаптивные алгоритмы, такие как bcrypt.  

---

</details>

