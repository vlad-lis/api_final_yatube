# yatube api

API проекта yatube.

Основной функционал: создание постов пользователями и добавление к ним комментариев.

## Локальный запуск проекта
1. Клонировать репозиторий.  
2. Установить зависимости: ```$ pip install -r requirements.txt```. 
3. Выполнить миграции ```$ python manage.py migrate``` 
3. Запустить проект ```$ python manage.py runserver```.

## Примеры запросов
- Список всех постов:
```
GET http://127.0.0.1:8000/api/v1/posts/
```

- Отдельный пост:
```
GET/POST/PUT/PATCH/DELETE http://127.0.0.1:8000/api/v1/posts/1/
```

- Комментарий к посту:
```
GET/POST http://127.0.0.1:8000/api/v1/posts/1/comments/
```
