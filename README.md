# Gesture Control Project

## Описание проекта

Этот проект предназначен для разработки системы управления с помощью жестов. В рамках проекта планируется создание системы, использующей компьютерное зрение для распознавания жестов руки и их интерпретации в действия, управляющие ПК. На данный момент реализована только структура проекта и начальная настройка окружения, в том числе часть, связанная с подготовкой инфраструктуры для машинного обучения.

## Структура проекта

Проект состоит из нескольких папок:

- **backend**: Логика распознавания и управления.
  - **models**: Модели машинного обучения и их обработка.
    - **trained_model**: Обученные модели.
    - **training_data**: Данные для обучения моделей.
  - **gesture_recognition**: Код распознавания жестов.
  - **utils**: Вспомогательные скрипты.
  - **main.py**: Главный файл запуска бэкенда.
  
- **interface**: Интерфейс управления ПК.
  - **assets**: Изображения, иконки, шрифты.
  - **views**: Окна и элементы GUI.
  - **controller**: Логика взаимодействия с бэкендом.
  - **main_interface.py**: Главный файл запуска интерфейса.
  
- **notebooks**: Jupyter Notebook для экспериментов.
  - **data_exploration.ipynb**: Анализ данных для обучения модели.
  - **model_training.ipynb**: Ноутбук для обучения и тестирования моделей.

- **README.md**: Документация.
- **requirements.txt**: Список зависимостей Python.

## Установка и настройка

Для того чтобы настроить проект на своем компьютере, следуйте следующим шагам.

1. **Клонируйте репозиторий:**
   
   Для начала клонируйте репозиторий с помощью команды:

   `git clone https://github.com/Grandelle/gesture_control_project.git`

2. **Создайте виртуальное окружение:**

   Перейдите в директорию проекта и создайте виртуальное окружение с помощью Python 3.10:

   `py -3.10 -m venv .venv` // конкретная версия 3.10.10


3. **Активируйте виртуальное окружение:**

   После создания виртуального окружения активируйте его:

   - Для Windows (PowerShell):
     `.venv\Scripts\Activate.ps1`

   - Для Windows (Command Prompt):
     `.venv\Scripts\activate`

   - Для Mac/Linux:
     `source .venv/bin/activate`

4. **Установите зависимости для ML:**

   В данный момент проект настроен только для работы с библиотеками машинного обучения. Для установки необходимых зависимостей выполните команду:

   `pip install -r requirements.txt`

## Зависимости

Проект использует следующие библиотеки:

- **opencv-python**: для работы с компьютерным зрением.
- **mediapipe**: для распознавания жестов с помощью модели.
- **tensorflow**: для работы с моделями машинного обучения.
- **flask**: для создания веб-сервера и API.

Эти библиотеки перечислены в файле `requirements.txt`.

## Возможности на будущее

В будущем проект может быть расширен следующими возможностями:

- Разработка системы распознавания жестов с помощью машинного обучения.
- Создание интерфейса для управления ПК с использованием жестов.
- Обучение более точных моделей для распознавания жестов.
- Оптимизация работы системы для более быстрого отклика и уменьшения задержек.

