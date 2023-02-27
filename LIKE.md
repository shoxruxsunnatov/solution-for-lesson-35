# Task 1
```sql
SELECT * FROM salesman
WHERE city = 'Paris' OR city = 'Rome';
```
![image](https://user-images.githubusercontent.com/81769242/221506448-67fb7290-20e0-4492-9f20-14643505c6b3.png)


# Task 2
```sql
SELECT * FROM salesman
WHERE city IN ('Paris','Rome');
```
![image](https://user-images.githubusercontent.com/81769242/221506582-17a6779f-39a9-4a32-82ac-2ba2d05539d8.png)


# Task 3
```sql
SELECT * FROM salesman
WHERE NOT city IN ('Paris','Rome');
```
![image](https://user-images.githubusercontent.com/81769242/221506886-2007a4d6-61cd-43bc-817e-a24fc4197813.png)


# Task 4
```sql
SELECT * FROM customer 
WHERE customer_id IN (3007, 3008, 3009);
```
![image](https://user-images.githubusercontent.com/81769242/221507344-e3ed60d4-066b-4a93-a670-6c0fa80ec69e.png)


# Task 5
```sql
SELECT * FROM salesman
WHERE commission BETWEEN 0.12 AND 0.14;
```
![image](https://user-images.githubusercontent.com/81769242/221507498-2cdc4a95-b929-44e5-bdae-a20e5b1f9373.png)


# Task 6
```sql
SELECT * FROM orders
WHERE (purch_amt BETWEEN 500 AND 4000) AND NOT purch_amt IN (948.50, 1983.43);
```
![image](https://user-images.githubusercontent.com/81769242/221507648-dd6e32ad-511f-4952-b7aa-0a30dfda68a3.png)


# Task 7
```sql
SELECT * FROM salesman
WHERE name LIKE 'A%' OR name LIKE 'L%'
```
![image](https://user-images.githubusercontent.com/81769242/221509277-b01cd01b-eeeb-4805-a27e-935dafda9362.png)


# Task 8

```sql
SELECT * FROM salesman
WHERE name NOT BETWEEN 'A' and 'L';
```
![image](https://user-images.githubusercontent.com/81769242/221508026-d7d48222-6861-4882-af9d-7fdd026ab261.png)


# Task 9
```sql
SELECT * FROM customer
WHERE cust_name LIKE 'B%';
```
![image](https://user-images.githubusercontent.com/81769242/221508273-72078c10-ef42-4728-8ec4-b228b7058051.png)


# Task 10
```sql
SELECT * FROM customer
WHERE cust_name LIKE '%n';
```
![image](https://user-images.githubusercontent.com/81769242/221508435-00c35c1b-1fed-4846-9542-585e0e91d901.png)


