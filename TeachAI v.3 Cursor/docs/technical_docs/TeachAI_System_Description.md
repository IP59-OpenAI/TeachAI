# Описание работы системы (ОРС)

## 1. Основные функции
- Сбор данных о пользователе.
- Генерация уроков и тестов через OpenAI.
- Контроль знаний с подсветкой ответов.
- Хранение прогресса и логов взаимодействий.

## 2. Логика работы

### 2.1. Первый запуск
1. Проверка `.env` и ключа API.
2. Настройка профиля пользователя:
   - Имя, время обучения, формат общения.
3. Сохранение данных в `state.json`.

### 2.2. Обучение
1. Вывод урока с использованием интерактивного интерфейса.
2. Генерация тестов и проверка знаний.
3. Сохранение результатов.

### 2.3. Повторное обучение
- Пользователь может возвращаться к предыдущим урокам или пропускать их.

### 2.4. Завершение курса
- После завершения всех уроков:
  - Отображается средний балл.
  - Логируется завершение курса.

## 3. Диагностика
- На каждом этапе проверяется корректность данных и действий.
- Отладочные сообщения выводятся в консоль и лог-файлы.
