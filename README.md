# Анализ данных транзакций

## Обзор проекта

Этот мини-проект направлен на анализ данных о транзакциях пользователей с целью получения информации о статусах транзакций и поведении пользователей. Набор данных `transaction_data.csv` содержит записи о транзакциях с деталями о датах, именах пользователей и статусах транзакций.

## Задачи

1. Загрузить набор данных и провести начальное исследование для понимания его структуры.
   - Проверить размер таблицы, типы данных, количество пропущенных значений и описательную статистику.
   
2. Проанализировать колонку `transaction`:
   - Определить уникальные значения и подсчитать количество наблюдений для каждого статуса.
   - Визуализировать результаты с помощью барплота и рассмотреть улучшения для большей ясности.

3. Определить количество транзакций, завершившихся ошибкой.

4. Подсчитать количество успешных транзакций для каждого пользователя:
   - Создать гистограмму для визуализации распределения успешных транзакций.

5. Когда будут получены обновленные данные от коллеги:
   - Построить сводную таблицу (`user_vs_minute_pivot`), где пользователи будут представлены в качестве столбцов, минуты — в качестве строк, а значения — количеством транзакций в указанную минуту. Заполнить пропущенные значения нулями.

6. Оценить предоставленный график, чтобы выяснить, есть ли в данных ошибка, или же всё в порядке.

7. Если в данные закралась ошибка, исправить её и сохранить правильное количество минут, прошедших с начала дня, в колонку `true_minute`.

## Описание данных

Набор данных включает в себя следующие колонки:
- **date**: Дата и время транзакции (в формате `YYYY-MM-DD HH:MM:SS`).
- **name**: Имя пользователя, инициировавшего транзакцию.
- **transaction**: Статус транзакции (например, успешная, ошибка).
- **minute**: Количество минут, прошедших с начала дня.

# Transaction Data Analysis

## Project Overview

This mini-project focuses on analyzing user transaction data to gain insights into transaction statuses and user behavior. The dataset `transaction_data.csv` contains records of transactions with details about dates, user names, and transaction statuses.

## Objectives

1. Load the dataset and conduct an initial exploration to understand its structure:
   - Verify the table's size, data types, number of missing values, and descriptive statistics.

2. Analyze the `transaction` column:
   - Identify unique values and count the number of observations for each status.
   - Visualize the results using a bar plot and consider improvements for better clarity.

3. Determine the number of transactions that resulted in errors.

4. Count the number of successful transactions for each user:
   - Create a histogram to visualize the distribution of successful transactions.

5. Upon receiving updated data from a colleague:
   - Build a pivot table (`user_vs_minute_pivot`), where users are represented as columns, minutes as rows, and values as the number of transactions in the specified minute. Fill missing values with zeros.

6. Evaluate the provided graph to determine if there is an error in the data or if everything is correct.

7. If an error exists, correct it and save the correct number of minutes passed since the start of the day in the `true_minute` column.

## Data Description

The dataset includes the following columns:
- **date**: Date and time of the transaction (formatted as `YYYY-MM-DD HH:MM:SS`).
- **name**: Name of the user who initiated the transaction.
- **transaction**: Transaction status (e.g., successful, error).
- **minute**: Number of minutes passed since the start of the day.
