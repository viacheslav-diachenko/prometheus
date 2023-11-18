**Coding Session - програмування телеграм бота на мові Golang**

Це завдання доволі популярне для новачків, оскільки воно дозволяє отримати базові навички програмування на Golang та використання API для взаємодії зі сторонніми сервісами. Успішне виконання даного завдання допоможете перейти до більш складних задач у розробці програмного забезпечення, а також сприяє підготовці до виконання творчого завдання.

**Ви отримали Технічне Завдання** на розробку функціонального Telegram-бота з кореневою командою та налаштуваннями. Він матиме можливість обробляти повідомлення від користувачів та відповідати на них:

* Мова Golang
* Фреймворки github.com/spf13/cobra та gopkg.in/telebot.v3
* Реалізувати обробники повідомлень для бота, які будуть відповідати на повідомлення в Telegram.
* Створити функції-обробники повідомлень бота.
* Додати ці функції до методів об'єкта telebot.Bot.
* Обробляти повідомлення відповідно до їх типу та вмісту.
 
**Це завдання дозволить вам:**

1. Ознайомитися з основними поняттями та функціями мови Golang.
2. Ознайомитися з Telegram Bot API та вивчити як його використовувати для розробки телеграм бота.
3. Навчитися створювати та налаштовувати бота для взаємодії з користувачами в телеграмі.
4. Практикувати знання з програмування та збільшити свій досвід у розробці програмного забезпечення.
5. Зрозуміти потреби та вимоги розробників до інфраструктури.

**Рекомендації до виконання:**

1. Встановити Golang та налаштувати середовище розробки (Codespaces вже містить всі необхідні налаштування)
2. Створити новий проєкт на GitHub та налаштувати Git.
3. Додати залежність на бібліотеку github.com/spf13/cobra за домопогою import (практичне завдання продемонстровано в лекції 2.4)
4. Створити Telegram-бота за допомогою BotFather.
5. Отримати токен бота та зберегти його у змінну середовища TELE_TOKEN.
6. Імпортувати необхідні бібліотеки.
7. Встановити бібліотеку gopkg.in/telebot.v3 за допомогою go get.
8. Отримати токен бота зі змінної середовища.
9. Створити об'єкт бота за допомогою telebot.NewBot().
10. Додати обробник повідомлень за допомогою kbot.Handle(telebot.OnText, func(m telebot.Context)
11. Описати функцію-обробник, яка буде відповідати на повідомлення.
12. Зібрати, запустити та перевірити бота
13. Створити файл README з описом проєкту, посиланням на бота у форматі t.me/<Імʼя_бота>_bot, включаючи інструкції для встановлення та приклади використання команд.
14. Завантажити код на GitHub.
15. Надіслати посилання на репозиторій як відповідь

**Якщо щось піде не так:**

1. Закомітьте поточний код до репозиторію;
2. Зверніться за допомогою у чат, надавши посилання та опис проблеми.

**Очікуваний практичний результат:**

* створено початковий код виконання практичного завдання
* перевірений працюючий код закомічено у репозиторій