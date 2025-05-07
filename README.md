Работаем и зарабатываем 📊⏰💰
Веб-приложение для учета рабочего времени и автоматического расчета заработка для студентов, фрилансеров и работников с гибким графиком.

🌟 Основные возможности
📅 Учет смен с детализацией (тип работы, дата, время, ставка)
🧮 Автоматический расчет заработка (почасовая оплата, премии)
📊 Визуализация данных (графики доходов по периодам)
🔔 Уведомления о предстоящих сменах
📱 Адаптивный интерфейс для всех устройств
🔒 Безопасная аутентификация через JWT

🛠 Технологический стек
Frontend:
Bootstrap 5 (адаптивный дизайн)
Vanilla JavaScript (работа с API, динамика)

Backend:
Django 5.2 + Django REST Framework
MySQL (основная БД) / SQLite (для разработки)
JWT-аутентификация

Инфраструктура:
Nginx + Gunicorn (продакшен)
Возможность деплоя на Heroku

📂 Структура проекта
workearn/
├── shifts/              # Основное приложение
│   ├── models.py        # Модели данных
│   ├── serializers.py   # Сериализаторы для API
│   ├── views.py         # Логика представлений
│   └── urls.py          # Маршруты API
├── templates/           # HTML-шаблоны
├── static/              # Статические файлы (JS/CSS)
└── workearn/            # Настройки проекта

🚀 Быстрый старт
Клонировать репозиторий:
git clone https://github.com/ваш-username/работаем-и-зарабатываем.git
cd workearn

Установить зависимости:
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt

Настроить БД (MySQL):
CREATE DATABASE workearn_db CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
CREATE USER 'ваш_пользователь'@'localhost' IDENTIFIED BY 'ваш_пароль';
GRANT ALL PRIVILEGES ON workearn_db.* TO 'ваш_пользователь'@'localhost';
FLUSH PRIVILEGES;

Запустить сервер:
python manage.py migrate
python manage.py runserver
Откройте http://localhost:8000 в браузере.
