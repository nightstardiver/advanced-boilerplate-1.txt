# Учебный шаблон проекта Portfolio

> Перед установкой зависимостей и запуском проекта убедитесь, что у вас установлена [последняя версия Node.js & NPM](https://nodejs.org/en/download/current/)

##  Чтобы развернуть проект необходимо:
```sh
$ git clone git@github.com:loftschool/advanced-boilerplate.git
$ cd advanced-boilerplate
$ npm install
```

## Скрипты package.json:

| Скрипт | Назначение |
| ------ | ------ |
| dev:mpa | Разработка основного сайта. Страницы **обо мне**, **блог** и т.п. Запустит dev сценарии **Gulp**. |
| dev:spa | Разработка админ панели в стиле **SPA** на **Vue.js** |
| build  | Сборка обоеих частей проекта. Все файлы будут доступны из директории **dist** |
| reg | Консольная утилита для регистрации. Использовать перед началом работы над **админ-панелью**. |

#### Чтобы запустить скрипт:
```sh
$ npm run имя_скрипта
```
У вас много ошибок, поэтому файл pug не может скомпилироваться в html
blog скомпилился, потому что в нем нет ошибок.
Нужно все исправить, тогда все заработает
pug_mixins.socials is not a function Где у вас объявляется этот миксин? Разберитесь в ошибках и все получится. Удачи :)

[18:36:22] Plumber found unhandled error: Говорит Plumber, что у вас ошибка
 TypeError in plugin "gulp-pug" Ошибка в плагине pug
Message:    Сообщение ошибки
    E:\advanced-boilerplate\src\views\pages\index.pug:14    Файл в котором ошибка
    12|             .user__info Личный сайт разработчика
    13|       .auth-block__socials
  > 14|         +socials(['vk', 'fb', 'in'], 'socials_fill_green')  > указывает на строку, в которой ошибка
    15|         .welcome__info Мои работы
    16|         .welcome__info Обо мне
    17|         .welcome__info Блог

pug_mixins.socials is not a function    Сама ошибка
Details:    Детали
    path: E:\advanced-boilerplate\src\views\pages\index.pug     Находятся в этом файле

    Это к примеру. Дальше сами попробуйте разобраться по образу и подобию