# Django Blog
Блог, разработанный с использованием Django фреймворка.

## Функционал:
- Регистрация пользователей с помощью электронной почты и пароля
- Возможность авторизации для зарегистрированных пользователей
- Создание, редактирование и удаление постов блога
- Отображение списка всех постов с возможностью поиска и фильтрации
- Комментирование постов
- Поддержка пагинации для длинных списков постов
- Автоматическое форматирование текста с использованием Markdown

## Технологии:
- Python
- Django
- HTML/CSS
- Bootstrap
- База данных PostgreSQL
- DRF

Запуск приложения
------
1. Склонируйте репозиторий:
```
git clone https://github.com/timoshenkost/django_blog
```

2. Перейдите в директорию проекта:
```
cd django_blog
```

3. Создайте виртуальное окружение и активируйте его:
```
python -m venv venv
source venv/bin/activate  # для Linux/Mac
venv\Scripts\activate  # для Windows
```

4. Установите зависимости:
```
pip install -r requirements.txt
```

5. Создайте в корне файл `.env` и запишите следующие поля:
```
GITHUB_KEY = 
GITHUB_SECRET = 

GOOGLE_KEY = 
GOOGLE_SECRET = 

SECRET_KEY = 

EMAIL_HOST = 
EMAIL_HOST_PASSWORD = 

DATABASE_PASSWORD = 
```

6. Выполните миграции базы данных:
```
python manage.py migrate
```

7. Для использования админ панели cоздайте суперпользователя:
```
python manage.py createsuperuser
```

8. Запустите сервер:
```
python manage.py runserver
```

Проект будет доступен по адресу http://localhost:8000/
