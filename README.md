🚀 Data Engineering Pet Project

📌 Описание

Этот проект — учебный кейс по Data Engineering, в котором реализован полный ETL-пайплайн (Extract, Transform, Load).
Проект собирает данные из нескольких источников, обрабатывает их и загружает в хранилище данных.

🏗 Архитектура

Источники данных: API, CSV-файлы, базы данных

ETL-процесс:

Extract: Получение и загрузка данных

Transform: Очистка, нормализация, агрегация

Load: Загрузка в Clickhouse/PostgreSQL

Хранилище данных: Clickhouse/PostgreSQL

Визуализация: Метрики и графики в Metabase

⚙️ Используемые технологии

🐍 Python (Pandas, Airflow, SQLAlchemy)

🐘 PostgreSQL / Clickhouse

🐳 Docker & Docker Compose

🎛 Apache Airflow (оркестрация)

📊 Metabase (визуализация)

📂 Структура проекта

├── dags/                 # DAG-файлы для Airflow
├── data/                 # Входные данные (если используются файлы)
├── db/                   # SQL-скрипты для схем БД
├── scripts/              # Скрипты для ETL
├── docker-compose.yml    # Конфигурация контейнеров
└── README.md             # Описание проекта

🚀 Запуск проекта

1️⃣ Установить зависимости

pip install -r requirements.txt

2️⃣ Запустить контейнеры

docker-compose up -d

3️⃣ Запустить DAG в Airflow

Перейти в Airflow UI и активировать DAG.

📊 Просмотр данных

После успешного выполнения ETL можно анализировать данные в Metabase (http://localhost:3000) или напрямую через SQL-запросы.

🎯 Возможные улучшения

Добавить поддержку Kafka для потоковой обработки

Автоматизировать CI/CD пайплайн для деплоя

Добавить мониторинг метрик (Prometheus + Grafana)

📧 Обратная связь

Если у тебя есть идеи или вопросы, пиши в Issues! 🚀

