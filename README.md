# lesson2

1.Открыл две консоли 

2.Сделать в первой сессии новую таблицу, наполнил данными

3.Посмотреть текущий уровень изоляции

postgres=# show transaction isolation level;

 transaction_isolation
-----------------------
 read committed
(1 row)

4.В первой сессии добавил новую запись

5.Сделал запрос на выбор всех записей во второй сессии

6.Вижу новую запись, потому что

7.Завершил транзакцию в первом окне

8.Сделал запрос на выбор всех записей второй сессии

9.Вижу новую запись

10.Завершил транзакцию во второй сессии

11.Начал repeatable read в обоих сессиях

12.В первой сессии добавил новую запись

13.Сделал запрос на выбор всех записей во второй сессии

14.Вижу новую запись

15.Завершил транзакцию в первом окне

16.Сделал запрос во выбор всех записей во второй сессии

17.Вижу новую запись
