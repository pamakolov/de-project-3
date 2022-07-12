# Проект 3

## Порядок выполнения

1. Обновление структуры таблицы staging.user_order_log,
добавляя новое поле status со значением по умолчанию "shipped".
файл update_staging.user_order_log.sql
   
2. Создание дополнительного скрипта на удаление данных из staging.user_order_log
на дату пробега DAG для получения идемпонентности.
файл - staging.user_order_log_delete_date.sql
   
3. Обновление кода заливки данных в mart.f_sales,
прописывая отрицательные значения для статуса "refunded", а также
перезаписывая данные на определенную дату.
файл update_mart.f_sales.sql
   
4. Создание таблицы-витрины mart.f_customer_retention.
файл mart.f_customer_retention.sql

5. Построение кода-скелета логики расчета витрины mart.f_customer_retention
с необходимыми полями
файл mart.f_customer_retention.sql
   
6. Добавление 2х новых тасков в DAG для запуска mart.f_customer_retention.sql
и удаления старых данных из staging.user_order_log
