# ToDo
веб-менеджер задач на django с использованием фреймворка semantic UI
___
создаем папку ToDo и переходим в неё
> mkdir ToDo & cd ToDo

устанавливаем виртуальное окружение
> python -m venv venv

активируем виртуальное окружение
>. venv/Scripts/activate

устанавливаем django
>pip install django

создаём проект todoapp и переходим в него
>django-admin startproject todoapp & cd todoapp

создаём приложение todolist
>python manage.py startapp todolist

Зарегистрируем приложение в файле settings.py

>INSTALLED_APPS = [

>...,

>todolist,
>
]

Укажем локализацию и часовой пояс в файле settings.py
>LANGUAGE_CODE = 'ru-ru'

>TIME_ZONE = 'Europe/Moscow'

Добавим папку шаблонов в settings.py

>TEMPLATES = [

>{...,

>'DIRS': ['templates'],

>}]

Создаем файл с зависимостями проекта
>pip freeze > requirements.txt

Запускаем сервер
>python manage.py runserver


#### p.s. после удачного создания проекта попробую упаковать его в docker контейнер...

