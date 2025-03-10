# Требования к курсовому проекту по курсу Анализ Данных

## Цель проекта
Создание интерактивного дашборда и его деплой на облачном хостинге Render. По итогам проекта студенты должны предоставить:
- ссылку на задеплоенный и работающий дашборд
- ссылку на репозиторий в котором хранится код проекта

## Используемые данные
- студенты должны самостоятельно выбрать датасет, который будет использоваться для создания дашборда
- студенты могут использовать публично доступные датасеты из интернета либо создать свой собственный датасет
- датасет должен состоять из минимум 3 таблиц, которые можно связать друг с другом по основным и внешним ключам


## Структура репозитория
В репозитории обязательно наличие:
- readme.md - файл с описанием репозитория. Должен содержать:
- название проекта и его краткое описание: кем создан, для чего и т.д.
- описание используемых инструментов
- описание структуры репозитория
- source (далее источник) - папка в которой должны хранится файлы используемого датасета в виде файлов с расширением .csv или .xlsx
- queries - папка, которая должна содержать файлы с расширением .sql, в которых должны содержаться:
- скрипт создания таблиц в базе данных (далее БД)
- скрипты создания представлений (далее вьюшки)
- скрипты запросов к вьюшкам
- my.db - локальный файл БД DuckDB
- ddl.py - модуль отвечающий за создание таблиц в БД и заполнение их данными из источника
- connector.py - модуль отвечающий за создание подключения к БД
- etl.py - модуль отвечающий за получение данных из БД для создания датафреймов
- dashboard.py - модуль отвечающий за создание дашборда


## readme.md
Файл с описанием репозитория. Должен содержать:
- название проекта и его краткое описание: кем создан, для чего и т.д.
- описание используемых инструментов
- описание структуры репозитория


## queries

Папка, которая должна содержать файлы с расширением .sql, в которых должны содержаться:
- скрипт создания таблиц в базе данных (далее БД)
- скрипты создания представлений (далее вьюшки)
- скрипты запросов к вьюшкам

## dashboard.py

Модуль отвечающий за создание дашборда