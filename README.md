# CI и CD проекта api_yamdb

![example event parameter](https://github.com/Alexandra1624/yamdb_final/actions/workflows/yamdb_workflow.yml/badge.svg?event=push)
## _Описание_
Для приложения **YaMDb** (https://github.com/Alexandra1624/api_yamdb) настроены Continuous Integration и Continuous Deployment. Реализовано:
- проверка кода на соответствие стандарту **PEP8** (с помощью пакета **flake8**) и запуск **pytest** из репозитория **yamdb_final**;
- сборка и доставка докер-образа для контейнера **web** на **Docker Hub**;
- автоматический деплой проекта на боевой сервер;
- отправка уведомления в **Telegram** о том, что процесс деплоя успешно завершился.

## Технологии
- Python 3.7.9
- Django 2.2.16
- Django Rest Framework 3.12.4
- Djangorestframework Simplejwt 5.1.0

## Установка
1. **Клонируйте репозиторий:**
```sh
git clone https://github.com/Alexandra1624/yamdb_final
```

2. **Cоздать и активировать виртуальное окружение:**
```sh
python -m venv venv
source venv/Scripts/activate
```

3. **Обновить pip и установить зависимости из файла requirements.txt:**
```sh
python -m pip install --upgrade pip
pip install -r requirements.txt
```

4. **Выполнить миграции:**
```sh
cd yatube_api
python manage.py migrate
```

5. **Создать суперпользователя:**
```sh
python manage.py createsuperuser
```

6. **Проверка тестов:**
```sh
pytest
```

7. **Запустить проект:**
```sh
python manage.py runserver
```
Сервер запущен на странице:     
http://localhost:8000       
Спецификация и эндпоинты доступны в документации:       
http://localhost:8000/redoc/

## Авторы

**_Александра Радионова_**      
https://github.com/Alexandra1624        
https://t.me/alexandra_R1624        
sashamain@yandex.ru