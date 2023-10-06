# Лабораторная работа №1. "Основы работы с Git и GitHub. Установка и настройка среды разработки Android Studio"
## Основы работы с Git и GitHub
### Установка и настройка Git
1. Скачайте дистрибутив Git с сайта https://git-scm.com/
2. Выполните установку. 
3. Добавьте путь к исполняемому файлу git в переменную среды PATH.
4. Проверьте, что команда ```git``` доступна из интерпретатора командной строки cmd.exe.
5. Установите имя пользователя и email с помощью команд.
```bash
  git config --global user.name "Name Surname"
  git config --global user.email "name@mail.ru"
```

### Регистрация и настройка GitHub
1. Перейдите на сайт https://github.com
2. Выполните регистрацию на сайте
3. Выполните fork репозитория https://github.com/chebotarevsa/mad-2023-lab01
4. В разделе **Settings > Developer Settings > Personal Access Tokens > Tokens (classic)** сгенерируйте новый токен.
  Для токена установите следующие параметры:
  + Name - Android Studio GitHub integration plugin
  + Expiration - No Expiration
  + Дать доступ для следующих Scope: repo, workflow, gist, admin:org/read:ord
5. Сохраните сгенеренный токен

### Работа с репозиторием
1. Выполните клонирование **своего** репозитория на локальную машину с помощью команды ```git clone <путь к репозиторию>```
2. Выполните команду ```git branch```. Объясните результат.
3. Создайте новую ветку с помощью команды ```git checkout -b fill_report```
4. Выполнить команду ```git branch```. Объясните результат.
5. Заполните раздел "Цель работы" в файле [REPORT.md](./REPORT.md)
6. Выполните команду ```git status```. Объясните результат.
7. Выполните команду ```git add REPORT.md```
8. Выполните команду ```git status```.  Объясните результат.
9. Выполните команду ```git commit -a -m "<Ваш комментарий>"``` для фиксации изменений
10. Выполните команду ```git status```.  Объясните результат.
11. Перейдите в ветку main. Проверьте файл  [REPORT.md](./REPORT.md). Объясните результат
12. Выполните слияние ветки  fill_report в ветку main c помощью команды ``` git merge fill_report ```
13. Выполните команду ```git log```. Объясните результат.
14. Удалите ветку fill_report с помощью команды  ```git branch --delete fill_report```
15. Проверьте, что ветка fill_report удалена
16. Отправьте изменения на сервер GitHub c помощью команды ```git push```. В качестве пароля используйте токен.

### Дополнительные материалы
+ Чакон, Страуб: Git для профессионального программиста. Питер, 2019 г.
+ https://git-scm.com/book/ru/v2  

## Установка и настройка среды разработки  Android Studio
1. Скачайте дистрибутив Android Studio c сайта https://developer.android.com/studio
2. Выполните установку
3. Запустите Android Studio и выполните шаги первичной настройки
4. Откройте в Android Studio директорию mad-2023-lab01. Откройте файл [REPORT.md](./REPORT.md).
5. Откройте меню **Help > Find Action** и введите "Choose Boot Java Runtime for the IDE…". 
Выполните команду. В открывшемся диалоговом окне выберите JRE "...with JCEF". Перезапустите Android Studio.
Данная настройка позволит в Android Studio удобно работать с языком разметки Markdown
6. Откройте пункт меню **File > Settings** выберите раздел **Version Control > Git**. Укажите путь к git.
7. Откройте пункт меню **File > Settings** выберите раздел **Version Control > GitHub**. Настройте доступ к своей учетный записи GitHub.
8. Заполните  разделы  "Выполнение работы" и "Вывод" [REPORT.md](./REPORT.md), где кратко опишите проделанную работу и сформулируйте вывод, соответственно.
9. Выполите фиксацию изменений в git и отправьте их на GitHub использую инструменты работы с git интегрированные в Android Studio.
  + Commit - пункт меню **Git > Commit**
  + Push - пункт меню **Git > Push**
  + Pull Request - пункт меню **Git > GitHub > Create Pull Request**
10. Создайте Pull Request в репозиторий [chebotarevsa/mad-2023-lab01](https://github.com/chebotarevsa/mad-2023-lab01). В названии Pull Request укажите группу и свою имя и фамилию, например "123 Иван Иванов".

### Дополнительные материалы
+ https://www.jetbrains.com/help/idea/using-git-integration.html

Срок сдачи работы до 11.10.2023
