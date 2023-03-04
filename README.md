Описание проекта.
В данном проекте реализована социальная сеть для обмена личной информацией и картинками.

Технологии.
Python, Django, DRF, Simple JWT.

Как запустить проект.

Клонировать репозиторий и перейти в его папку в командной строке:

git clone https://github.com/AnastasiyaGuchek/api_final_yatube.git
cd api_final_yatube
Cоздать и активировать виртуальное окружение:

python -m venv venv

Для *nix-систем:
source venv/bin/activate

Для windows-систем:
source venv/Scripts/activate

Установить зависимости из файла requirements.txt:

python -m pip install --upgrade pip
pip install -r requirements.txt

Выполнить миграции:
cd yatube_api
python manage.py migrate

Создать суперпользователя django:
python manage.py createsuperuser

Запустить проект:
python manage.py runserver

Разработчик
Анастасия Гучек