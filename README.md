# bookmarks

## Проект социальной сети
Приложение, которое дает пользователям возможность делиться фотографиями и картинками, которые они нашли в интернете.

* В проекте реализована возможность аутентификации, для того чтобы пользователи могли регестрироваться в соцсети, заходить под своим аккаунтом, редактировать профиль и менять пароль.

* Реализована система подписок, чотбы пользователи могли наблюдать за обновлениями, происходящими у друзей.

* Отображение картинок, которыми делятся пользователи.

* Лента для каждого пользователя, чтобы каждый мог видеть обновления у тех, на кого подписался.

## Запуск проекта в dev-режиме:
Инструкция ориентирована на операционную систему windows и утилиту git bash.<br/>
Для прочих инструментов используйте аналоги команд для вашего окружения.

1. Клонируйте репозиторий и перейдите в него в командной строке:

```
git clone https://github.com/SergeyViskov/bookmarks.git
```

```
cd bookmarks
```

2. Установите и активируйте виртуальное окружение
```
python -m venv venv
``` 
```
source venv/Scripts/activate
```

3. Установите зависимости из файла requirements.txt
```
pip install -r requirements.txt
```

4. В папке с файлом manage.py выполните миграции:
```
python manage.py migrate
```

5. В папке с файлом manage.py запустите сервер, выполнив команду:
```
python manage.py runserver
```