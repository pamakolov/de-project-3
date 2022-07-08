# Проект 3

## Порядок выполнения

1. Обновление структуры таблицы staging.user_order_log,
добавляя новое поле status со значением по умолчанию "shipped".
файл update_staging.user_order_log.sql
   
2. Обновление кода заливки данных в mart.f_sales,
прописывая отрицательные значения для статуса "refunded".
файл update_mart.f_sales.sql
   
3. Создание таблицы-витрины mart.f_customer_retention.
файл mart.f_customer_retention.sql

4. Построение кода-скелета логики расчета витрины mart.f_customer_retention
с необходимыми полями
файл mart.f_customer_retention.sql
