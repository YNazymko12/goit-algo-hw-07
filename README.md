# Домашнє завдання до теми “Дерева та балансування”

Готові до тренування? 🤩

Ви вже знаєте властивості двійкових дерев пошуку та основні операції, які можна
над такими деревами здійснювати, переваги та приклади їх застосування.

Сьогодні ви потренуєтесь працювати з двійковим деревами пошуку та
`AVL-деревами`, а саме писати функції для виконання різних завдань.

Домашнє завдання буде складатися з трьох незалежних обов’язкових завдань, а
також четвертого додаткового завдання за бажанням.

## Опис домашнього завдання

### Завдання 1

Напишіть алгоритм (функцію), який знаходить найбільше значення у двійковому
дереві пошуку або в `AVL-дереві`. Візьміть будь-яку реалізацію дерева з
конспекту чи з іншого джерела.

### Завдання 2

Напишіть алгоритм (функцію), який знаходить найменше значення у двійковому
дереві пошуку або в `AVL-дереві`. Візьміть будь-яку реалізацію дерева з
конспекту чи з іншого джерела.

### Завдання 3

Напишіть алгоритм (функцію), який знаходить суму всіх значень у двійковому
дереві пошуку або в `AVL-дереві`. Візьміть будь-яку реалізацію дерева з
конспекту чи з іншого джерела.

### Завдання 4 (необов'язкове завдання)

Реалізуйте структуру даних для системи коментарів так, щоб коментарі могли мати
відповіді, які, в свою чергу, також могли мати відповіді, формуючи таким чином
ієрархічну структуру.

Також візьміть до уваги наступні вимоги:

- Реалізуйте клас `Comment`, що представляє собою окремий коментар. Він має
  зберігати текст коментаря, автора та список відповідей.
- Метод класу `add_reply` має додавати нову відповідь до коментаря.
- Метод класу `remove_reply` має видаляти відповідь із коментаря. Це має
  змінювати текст коментаря на стандартне повідомлення (наприклад, "Цей коментар
  було видалено.") і встановлювати прапорець `is_deleted` в `True`.
- Метод `display` має рекурсивно виводити коментар та всі його відповіді,
  використовуючи відступи для відображення ієрархічної структури.

Приклад очікуваного результату:

```python
root_comment = Comment("Яка чудова книга!", "Бодя")
reply1 = Comment("Книга повне розчарування :(", "Андрій")
reply2 = Comment("Що в ній чудового?", "Марина")

root_comment.add_reply(reply1)
root_comment.add_reply(reply2)

reply1_1 = Comment("Не книжка, а перевели купу паперу ні нащо...", "Сергій")
reply1.add_reply(reply1_1)

reply1.remove_reply()

root_comment.display()
```

Виведення:

```python
Бодя: Яка чудова книга!
Цей коментар було видалено.
Сергій: Не книжка, а перевели купу паперу ні нащо...
Марина: Що в ній чудового?
```

## Підготовка та завантаження домашнього завдання

1. Створіть публічний репозиторій `goit-algo-hw-07`.

2. Виконайте завдання та відправте його у свій репозиторій.

3. Завантажте робочі файли на свій комп’ютер та прикріпіть їх у `LMS` у форматі
   `zip`. Назва архіву повинна бути у форматі `ДЗ7_ПІБ`.

4. Прикріпіть посилання на репозиторій `goit-algo-hw-07` та відправте на
   перевірку.

> [!IMPORTANT]
>
> 💡 ВАЖЛИВО Перегляньте Інструкцію щодо завантаження робочого файлу з
> репозиторію на Github

## Формат здачі

- Прикріплені файли репозиторію у форматі `zip` з назвою `ДЗ7_ПІБ`.
- Посилання на репозиторій.

## Критерії прийняття ДЗ

Прикріплені посилання на репозиторій `goit-algo-hw-0`7 та безпосередньо самі
файли репозиторію у форматі `zip`.

### Завдання 1:

Код виконується, і функція знаходить найбільше значення в дереві.

### Завдання 2:

Код виконується, і функція знаходить найменше значення в дереві.

### Завдання 3:

Код виконується, і функція знаходить суму всіх значень у дереві.

### Завдання 4 (необов'язкове завдання):

Завдання є додатковим, тому не оцінюється, проте, за бажанням, ви можете
отримати конструктивний зворотній зв’язок від ментора.

### Формат оцінювання

Оцінка від 0 до 100. Завдання 1 оцінюється в 30 балів. Завдання 2 оцінюється в
30 балів. Завдання 3 оцінюється в 40 балів. Завдання 4 є опціональним, тому не
оцінюється.
