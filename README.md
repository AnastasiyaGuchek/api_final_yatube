# Описание проекта

В данном проекте реализована социальная сеть для обмена личной информацией и картинками.

# Технологии
Python, Django, DRF, Simple JWT.

# Как запустить проект:

- Клонировать репозиторий и перейти в его папку в командной строке:
```
git clone https://github.com/AnastasiyaGuchek/api_final_yatube.
```
```
cd api_final_yatube
```
- Cоздать и активировать виртуальное окружение:
```
python -m venv venv
```
```
source venv/Scripts/activate
```
- Установить зависимости из файла requirements.txt:
```
pip install -r requirements.txt
```
- Выполнить миграции:
```
cd yatube_api
```
```
python manage.py migrate
```
- Создать суперпользователя django:
```
python manage.py createsuperuser
```
- Запустить проект:
```
python manage.py runserver
```
# Настроены такие эндпоинты:
- Пример POST-запроса http://127.0.0.1:8000/api/v1/posts/
- Пример ответа:
```
{
    "id": 2,
    "author": "root",
    "text": "Сегодня прекрасная погода",
    "pub_date": "2023-03-06T21:29:21.463128+03:00",
    "image": null,
    "group": null
}
```
- Пример GET-запроса http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/{id}/
- Пример ответа:
```
{
    "id": 1,
    "author": "root",
    "text": "Солнечно",
    "created": "2023-03-06T21:43:13.647282+03:00",
    "post": 2
}
```
- Пример POST-запроса http://127.0.0.1:8000/api/v1/jwt/create/
```
{
    "username": "string",
    "password": "string"
}
```
- Пример ответа:
```
{
    "refresh": "string",
    "access": "string"
}
```
# Разработчик
Анастасия Гучек