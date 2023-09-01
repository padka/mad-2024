# Лабораторная работа "Основы работы с Git и GitHub. Устанока и настрока среды разработки  Android Studio"
## Основы работы с Git и GitHub
### Установка и настройка Git
+ Скачать дистрибутив Git с сайта https://git-scm.com/
+ Выполнить установку. 
+ Добавить путь к исполняемому файлу git в переменную среды PATH.
+ Проверить что команда ```git``` доступна из интерпретатора командной строки cmd.exe.
+ Установить имя пользователя и email с помощью команд.
```bash
  git config --global user.name "Name Surname"
  git config --global user.email "name@mail.ru"
```
### Регистрация и настройка GitHub
+ Перейти на сайт https://github.com
+ Выполнить регистрацию на сайте
+ Выполнить fork репозитория https://github.com/chebotarevsa/mad-2023-lab01
+ В разделе **Settings -> Developer Settings -> Personal Access Tokens -> Tokens (classic)** сгенерировать новый токен.
  Для токена установить следующие параметры
  + Name - Android Studio GitHub integration plugin
  + Expiration - No Expiration
  + Дать доступ для следующих Scope: repo, workflow, gist, admin:org/read:ord
+ Сохранить сгенеренный токен

### Работа с репозиторием
+ Выполнить клонирование **своего** репозитория с помощью команды ```git clone <путь к репозиторию>```
+ Создать новую ветку с помощью команды 

### Дополнительная литература
+ Чакон, Страуб: Git для профессионального программиста. Питер, 2019 г.
+ https://git-scm.com/book/ru/v2  

## Устанока и настрока среды разработки  Android Studio
