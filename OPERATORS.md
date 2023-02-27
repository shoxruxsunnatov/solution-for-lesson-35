# Task 1
```sql
SELECT * FROM customer WHERE grade > 100;
```
![image](https://user-images.githubusercontent.com/81769242/221503089-c8b23940-0077-4e4f-afc5-8c467c4c6a92.png)

# Task 2
```sql
SELECT * FROM customer
WHERE city = 'New York' AND grade > 100;
```
![image](https://user-images.githubusercontent.com/81769242/221503320-2fda4e59-17ec-4f9a-8307-10f86265458d.png)


# Task 3
```sql
SELECT * FROM customer WHERE city = 'New York' OR grade > 100;
```
![image](https://user-images.githubusercontent.com/81769242/221503520-67b4c8dc-c06c-4bc9-bb22-b296f344b3a5.png)


# Task 4
```sql
SELECT * FROM customer WHERE city = 'New York' OR NOT grade > 100;
```
![image](https://user-images.githubusercontent.com/81769242/221503706-0addb374-a82d-41d2-83a5-2dd76150b903.png)


# Task 5
```sql
SELECT * FROM customer WHERE NOT (city = 'New York' OR grade > 100);
```
![image](https://user-images.githubusercontent.com/81769242/221503831-4730fc30-1aab-4b85-99d7-059e213ee4d5.png)


# Task 6
```sql
SELECT * FROM  orders 
WHERE NOT ((ord_date = '2012-09-10' AND salesman_id > 5005)
OR purch_amt > 1000.00);
```
![image](https://user-images.githubusercontent.com/81769242/221504402-9f71c7b2-29f5-417a-8b0f-850f03347d32.png)


# Task 7
```sql
SELECT
  salesman_id,
  name,city,
  commission
FROM salesman
WHERE (commission > 0.10 AND commission < 0.12);
```
![image](https://user-images.githubusercontent.com/81769242/221504577-183dec73-45f6-47b5-9913-a082c6268687.png)


# Task 8
```sql
SELECT * FROM  orders
WHERE (purch_amt < 200 OR NOT (ord_date >= '2012-02-10' AND customer_id < 3009));
```
![image](https://user-images.githubusercontent.com/81769242/221504808-16462188-c6db-48f8-8797-963f87e2e9d9.png)


# Task 9
```sql
SELECT * FROM  orders
WHERE NOT ((ord_date = '2012-08-17' OR customer_id > 3005) AND purch_amt < 1000);
```
![image](https://user-images.githubusercontent.com/81769242/221505091-72cd91e0-a675-452f-9b4b-c65c27bdabc7.png)


# Task 10
```sql
SELECT
  ord_no,
  purch_amt,
  (100 * purch_amt) / 6000 AS "Achieved %",
  (100 * (6000 - purch_amt) / 6000) AS "Unachieved %"
FROM  orders
WHERE (100 * purch_amt) / 6000 > 50;
```
![image](https://user-images.githubusercontent.com/81769242/221505426-c5f8615c-e256-4226-b93e-bf74691dea1c.png)


# Task 11
```sql
SELECT * FROM emp_details
WHERE emp_lname = 'Dosni' OR emp_lname= 'Mardy';
```
![image](https://user-images.githubusercontent.com/81769242/221505519-db499d5a-394d-49e4-8d78-f3c82e995c18.png)


# Task 12
```sql
SELECT * FROM emp_details
WHERE emp_dept = 47 OR emp_dept = 63;
```
![image](https://user-images.githubusercontent.com/81769242/221505662-cee50ab2-781f-4f3d-8000-cabc8d039cd9.png)


