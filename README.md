# luxmus_test
Test task for Luxmus organisation
# Задание №1
В этом задании предполагался анализ данных с использованием языка SQL и навыки владения им.
Я выполнил задания 1, 2, 3, 5. SQL выражения для данных заданий поместил в папку task_1/SQL answers.txt. 
К первому заданию приложен DDL, сформированный программой DBeaver.
Остальные задания содержать SQL выражения для вычисления необходимых таблиц.

# Задание №2
Хранится в папке task_2 и представляет собой скрипты для выгрузки данных из API и представления витрины данных для будущего дашборда, а также основной скрипт, соединяющий их воедино. 

## Системные требования
Язык для формирования ETL процесса - Python 3.11.6
База данных - SQLite3 

## Используемые библиотеки
SQLAlchemy==1.4.44
pandas==1.5.3
jupyterlab==4.0.10
json5==0.9.14
requests==2.31.0

## Использование программы через Jupyter Lab
1. Необходимо установить последнюю версию Python и установить необходимые библиотеки, перечисленные в requirements.txt;
2. Открыть jupyter-lab и открыть main.ipynb, в котором хранится основной скрипт программы;
3. Запустить все необходимые ячейки, что делает каждая ячейка описано в описание к соответствующей ячейке.

## Использование программы через консоль
1. Необходимо установить последнюю версию Python и установить необходимые библиотеки, перечисленные в requirements.txt;
2. Через командную строку запустить скрипт main.py.

## Возможные усовершенствования данного ПО
1. Добавление распаралелленых процессов, которые ускорят обращение к API и как следствие, ускорят обработку данного скрипта (multiprocessing);
2. Использование более современной базы данных (использование sqlite3 было обусловленно необходимостью хранения данных в файле для того, чтобы в дальнейшем было удобно проверить результаты);
3. Дополнение витрины данных для дашборда информацией относительно общего количества персонажей из различного вида происхождений.

## Структура проекта
api.py - класс для общения с API, данным в задании;
etl.py - класс, описывающий ETL-процесс, который происходит для формирования витрины данных;
main.ipynb - основной скрипт программы (версия для jupyter-lab);
main.py - основной скрипт программы (версия для консоли python);
sqlite3.db - база данных для проекта с таблицей earth_characters, где хранится витрина данных, необходимая для выполнения задания.
requirements.txt - зависимости, необходимые для корректной работы скрипта.
