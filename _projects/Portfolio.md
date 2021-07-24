---
layout: post
title: "Portfolio"
image: "/projects/portfolio.png"
image_alt: "Скриншот демо приложения"
---

Данное портфолио написано на phpc использования фреймворка Laravel, размещено на сервере и работает с базой данных MySql. 
Так же в нём установлен телеграмм бот BotFather который настроен на отправку мне личных сообщений.

![Скриншот](/assets/img/projects/portfolio.gif "Запсиь демо сайта")

Список того, что я использовал в этом проекте следующий:
- PHP
- Laravel
- BotFather
- MySql
- JS
- Bootstrap
- Html
- CSS

## Демо

Разместил я этот сайт-портфолио на бесплатном хостинге `000webhostapp.com` на [данной странице](https://evgenyyushko.000webhostapp.com/){:target="_blank"}{:rel="noreferrer"}.

## Как я это сделал

Для того чтоб сделать подобный сайт у вас должны быть установленн `git`, одна из `IDE`, `Php Shtorm` или хотя бы `VS Code`. Далее вы можете склонировать
себе репозиторий.

```bash
git clone git@github.com:EvgenyYushko/MyCV.git
```

В нём лежат начальные исходники этого проекта. Это пустая оболочка(каркас) написанный чисто на на `HTML` и `CSS`, выглядит он 
[следующим образом](https://evgenyyushko.github.io/MyCV/){:target="_blank"}{:rel="noreferrer"}. 

После того, как репозиторий будет склонирован, вам нужно будет установить фреймворк `Laravel` следующей командой 
`composer create-project laravel/laravel quickstart --prefer-dist`.

Далее перейти в php консоль, в папку с проектом и выполнить `composer install`.
Установиться папка `vendor` и загрузит фреймворк и подтянет все зависимости.

Создаст все наши таблицы БД `php artisan migrate`

Перейти в `C:\Windows\System32\drivers\etc` открыть файл `hosts` (admin right) прописать имя хоста `127.0.0.1 portfolio.loc`

Запустить сервер. Перейти в админку `portfolio.loc/admin` добавить раздел `/profile` добавить нового пользователя указав ему slug.

При необходимости выполнить `php artisan admin:install`