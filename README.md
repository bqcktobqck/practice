# Apache Log Aggregator
Описание
Приложение для агрегации данных из access логов веб-сервера Apache с сохранением в базу данных MySQL. Приложение позволяет просматривать сохраненные данные, фильтровать их по IP, дате и промежутку дат, а также предоставляет API для получения данных в формате JSON.

# Установка и настройка

Шаг 1: Клонирование репозитория

git clone https://github.com/bqcktobqck/practice.git
cd practice

Шаг 2: Установка зависимостей
Создайте виртуальное окружение и активируйте его:

python -m venv venv
source venv/bin/activate

Шаг 3: Установите зависимости

pip install -r requirements.txt

Шаг 4: Cоздание и миграция базы данных

flask db init
flask db migrate
flask db upgrade

Шаг 5: Нужно произвести настройку переменных окружений в .env файле

Шаг 6: Запуск приложения

python app.py

Тут будет доступ http://127.0.0.1:5000/.
