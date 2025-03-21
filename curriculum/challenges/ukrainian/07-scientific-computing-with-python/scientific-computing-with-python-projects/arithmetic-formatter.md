---
id: 5e44412c903586ffb414c94c
title: Арифметичний форматор
challengeType: 10
forumTopicId: 462359
dashedName: arithmetic-formatter
---

# --description--

Ви будете <a href="https://replit.com/github/freeCodeCamp/boilerplate-arithmetic-formatter" target="_blank" rel="noopener noreferrer nofollow">працювати над цим проєктом з нашим стартовим кодом Replit</a>.

-   Почніть з імпорту проєкту на Replit.
-   Потім ви побачите вікно `.replit`.
-   Оберіть `Use run command` та натисніть кнопку `Done`.


# --instructions--

У початковій школі вчать вирішувати математичні приклади вертикально, аби було простіше. Наприклад, «235 + 52» перетворюється на:

```py
  235
+  52
-----
```

Створіть функцію, яка отримує список рядків з математичними прикладами та послідовно повертає їх у вертикальному вигляді. В разі потреби функція повинна приймати другий аргумент. Коли другий аргумент встановлено на `True`, відповіді повинні відображатися.

## Наприклад

Виклик функції:

```py
arithmetic_arranger(["32 + 698", "3801 - 2", "45 + 43", "123 + 49"])
```

Вивід:

```py
   32      3801      45      123
+ 698    -    2    + 43    +  49
-----    ------    ----    -----
```

Виклик функції:

```py
arithmetic_arranger(["32 + 8", "1 - 3801", "9999 + 9999", "523 - 49"], True)
```

Вивід:

```py
  32         1      9999      523
+  8    - 3801    + 9999    -  49
----    ------    ------    -----
  40     -3800     19998      474
```

## Правила

Функція поверне правильне перетворення, якщо надані приклади відформатовані правильно. В іншому випадку буде **повернений** **рядок**, який описує помилку, важливу для користувача.


- Ситуації, які повернуть помилку:
  - Функції надано **забагато прикладів**. Ліміт складає **5 прикладів**. Якщо їх більше, то повернеться `Error: Too many problems.`
  - Функція приймає відповідні оператори: **додавання** та **віднімання**. Множення та ділення поверне помилку. Інші оператори, які не згадані тут, тестовані не будуть. Повернеться помилка `Error: Operator must be '+' or '-'.`
  - Кожне число (операнд) повинне містити лише цифри. В іншому випадку функція поверне `Error: Numbers must only contain digits.`
  - Кожен операнд (тобто число з кожної сторони оператора) може мати максимум чотири цифри по ширині. В іншому випадку помилковий рядок видасть `Error: Numbers cannot be more than four digits.`
- Якщо користувач надав правильний формат прикладу, то перетворення буде дотримуватись таких правил:
  - Повинен бути лише один пробіл між оператором і найдовшим із двох операндів; оператор буде на тому ж рядку, що й другий операнд; обоє операндів будуть в тому порядку, як і надано (перший буде зверху, а другий буде знизу).
  - Числа повинні бути вирівняні за правим краєм.
  - Між кожним прикладом повинно бути чотири пробіли.
  - Знизу кожного прикладу повинна бути риска. Риска повинна йти по всій довжині прикладу індивідуально. (На прикладі вище видно, як це повинно виглядати.)

## Розробка

Запишіть свій код у `arithmetic_arranger.py`. Для розробки ви можете використати `main.py`, щоб протестувати свою функцію `arithmetic_arranger()`. Натисніть кнопку «run» і `main.py` запуститься.

## Тестування

Модульні тести для цього проєкту знаходяться в `test_module.py`. Ми запускаємо тести з `test_module.py` в `main.py` для вашої зручності. Тести запустяться автоматично, коли ви натиснете на кнопку «run». Як варіант, ви можете запустити тести, ввівши `pytest` на консолі.

## Надсилання

Copy your project's URL and submit it to freeCodeCamp.

# --hints--

Проєкт повинен правильно відформатувати математичний приклад та пройти всі тести.

```js

```

# --solutions--

```js
/**
  Backend challenges don't need solutions,
  because they would need to be tested against a full working project.
  Please check our contributing guidelines to learn more.
*/
```
