# Task 1
```sql
SELECT SUM (purch_amt) FROM orders
```
![image](https://user-images.githubusercontent.com/81769242/221510126-b1021ba6-ac92-4163-87fd-05b2b0f74e78.png)

# Task 2
```sql
SELECT AVG (purch_amt) FROM orders
```
![image](https://user-images.githubusercontent.com/81769242/221510402-f5065b61-ed4e-4741-8472-556e29fe8be0.png)


# Task 3
```sql
SELECT COUNT (DISTINCT salesman_id) FROM orders
```
![image](https://user-images.githubusercontent.com/81769242/221510577-7300aac1-a1ba-4046-9392-a439d83959f5.png)


# Task 4
```sql
SELECT COUNT(*) FROM customer;
```
![image](https://user-images.githubusercontent.com/81769242/221510697-675f7f10-e821-4d77-be42-76875f6c50ba.png)


# Task 5
```sql
SELECT COUNT (grade) FROM customer
WHERE grade > 0
```
![image](https://user-images.githubusercontent.com/81769242/221513437-1812f9ed-10c8-4055-a77c-8bb3a210cb19.png)


# Task 6
```sql
SELECT MAX (purch_amt) FROM orders
```
![image](https://user-images.githubusercontent.com/81769242/221513648-da607b3b-fb9a-43f1-bfdb-ab54eef78790.png)


# Task 7
```sql
SELECT MIN(purch_amt) FROM orders
```
![image](https://user-images.githubusercontent.com/81769242/221513773-52a818fa-f60c-4e1d-8c4c-ccb8f8f5912c.png)


# Task 8
```sql
SELECT city, MAX (grade) FROM customer
GROUP BY city;
```
![image](https://user-images.githubusercontent.com/81769242/221513885-2c6600db-64c2-4ef2-8980-4eebcfbd7e4c.png)


# Task 9
```sql
SELECT customer_id, MAX (purch_amt) FROM orders
GROUP BY customer_id;
```
![image](https://user-images.githubusercontent.com/81769242/221514142-138bf45b-7a07-4b57-af80-7fdc43c6596e.png)


# Task 10
```sql
SELECT customer_id, ord_date, MAX (purch_amt) FROM orders
GROUP BY customer_id, ord_date;
```
![image](https://user-images.githubusercontent.com/81769242/221514277-b9f59075-43b2-4e54-9212-6d4406cd8778.png)

