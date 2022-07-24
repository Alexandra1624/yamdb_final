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


2. **Создайте файл .env с переменными окружения для работы с базой данных:**
```sh
SECRET_KEY=secret_key # секретный ключ для работы settings.py
DB_ENGINE=django.db.backends.postgresql # указываем, что работаем с postgresql
DB_NAME=postgres # имя базы данных
POSTGRES_USER=postgres # логин для подключения к базе данных
POSTGRES_PASSWORD=postgres # пароль для подключения к БД (установите свой)
DB_HOST=db # название сервиса (контейнера)
DB_PORT=5432 # порт для подключения к БД
```
Сервер запущен на странице:     
http://62.84.120.234       
Страница администратора:
http://62.84.120.234/admin
Спецификация и эндпоинты доступны в документации:       
http://62.84.120.234/redoc/

## Автор

**_Александра Радионова_**      
https://github.com/Alexandra1624        
https://t.me/alexandra_R1624        
sashamain@yandex.ru