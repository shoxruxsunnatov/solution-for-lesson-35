# Task 1
```sql
SELECT * FROM salesman
```
![image](https://user-images.githubusercontent.com/81769242/221484494-6ce33f13-b44a-4d1c-aaa6-2a862256e9b8.png)


# Task 2
```sql
SELECT 'This is SQL Exercise, Practice and Solution'
```
![image](https://user-images.githubusercontent.com/81769242/221484833-2395a3ef-9fdd-465e-b3a4-230724fd97ba.png)


# Task 3
```sql
SELECT 1, 2, 3
```
![image](https://user-images.githubusercontent.com/81769242/221492879-618af151-63e5-4a51-b9d5-274fc461ec70.png)


# Task 4
```sql
SELECT 30 + 20
```
![image](https://user-images.githubusercontent.com/81769242/221485228-4b0ee77e-a164-46a5-93fd-126235a04d84.png)


# Task 5
```sql
SELECT 30 + 20 * 2 / 3
```
![image](https://user-images.githubusercontent.com/81769242/221485389-673d61f7-0919-4bf5-bc42-f0312e541307.png)


# Task 6
```sql
SELECT name, commission FROM salesman;
```
![image](https://user-images.githubusercontent.com/81769242/221485868-62f19b93-f63c-4c3c-ac67-18b89ed27d30.png)


# Task 7
```sql
SELECT ord_date, salesman_id, ord_no, purch_amt FROM orders;
![image](https://user-images.githubusercontent.com/81769242/221485952-70aa0000-c1bd-4789-8a95-000c7f40ec72.png)

# Task 8
```sql
SELECT DISTINCT salesman_id FROM orders;
```
![image](https://user-images.githubusercontent.com/81769242/221486109-b5cdae55-24a2-4c4c-ab3b-67393c6848ba.png)


# Task 9
```sql
SELECT name,city FROM salesman WHERE city = 'Paris';
```
![image](https://user-images.githubusercontent.com/81769242/221486285-464bc790-2305-4762-ab8d-2e225e13f7e9.png)


# Task 10
```sql
SELECT *FROM customer WHERE grade = 200;
```
![image](https://user-images.githubusercontent.com/81769242/221486568-ddd5d1ac-fca4-405b-9d31-29235036cf32.png)


# Task 11
```sql
SELECT ord_no, ord_date, purch_amt FROM orders
WHERE salesman_id = 5001;
```
![image](https://user-images.githubusercontent.com/81769242/221486685-7881cc09-744a-4c5d-b56d-d55b85a536b1.png)


# Task 12
```sql
SELECT year,subject,winner FROM nobel_win
WHERE year = 1970; 
```
![image](https://user-images.githubusercontent.com/81769242/221487299-3f383421-d109-478e-b33e-fea2515d711e.png)


# Task 13
```sql
SELECT winner FROM nobel_win
WHERE year = 1971 AND subject = 'Literature';
```
![image](https://user-images.githubusercontent.com/81769242/221487434-ab4d3218-3e05-42dd-a2ad-b3005c995ef7.png)


# Task 14
```sql
SELECT year, subject FROM nobel_win
WHERE winner = 'Dennis Gabor';
```
![image](https://user-images.githubusercontent.com/81769242/221487668-11298ac8-146c-45d3-9ffc-de5768361529.png)


# Task 15
```sql
SELECT winner FROM nobel_win
WHERE year >= 1950 AND subject = 'Physics';
```
![image](https://user-images.githubusercontent.com/81769242/221487916-704a9d5a-366f-40c3-860b-cd9d4a76e10d.png)


# Task 16
```sql
SELECT year, subject, winner, country FROM nobel_win
WHERE subject = 'Chemistry' AND year >= 1965 AND year <= 1975;
```
![image](https://user-images.githubusercontent.com/81769242/221488192-1be3a8b0-708a-4afd-a7df-4cf1d15bcbbe.png)


# Task 17
```sql
SELECT * FROM nobel_win
WHERE year > 1972 AND winner IN ('Menachem Begin','Yitzhak Rabin');
```
![image](https://user-images.githubusercontent.com/81769242/221488531-2477d482-d847-4f73-8662-ede79b452d05.png)


# Task 18
```sql
SELECT * FROM nobel_win
WHERE winner LIKE 'Louis %';
```
![image](https://user-images.githubusercontent.com/81769242/221488701-2917d908-32e7-4152-880b-d42bf058bd28.png)


# Task 19
```sql
SELECT * FROM nobel_win
WHERE subject = 'Physics' and year = 1970
OR SUBJECT = 'Economics' and year = 1971
```
![image](https://user-images.githubusercontent.com/81769242/221489606-0b6ea9c9-4c18-452a-a698-aa209026fee8.png)


# Task 20
```sql
SELECT * FROM nobel_win
WHERE year=1970 AND subject NOT IN ('Physiology','Economics');
```
![image](https://user-images.githubusercontent.com/81769242/221489803-b165bd7f-dc57-4691-af46-684c0a96e71b.png)


# Task 21
```sql
SELECT * FROM nobel_win
WHERE subject = 'Physiology' AND year < 1971
OR subject = 'Peace' AND year >= 1974;
```
![image](https://user-images.githubusercontent.com/81769242/221490413-269a9570-85cd-4b53-99db-098940c5cc08.png)


# Task 22
```sql
SELECT * FROM nobel_win
WHERE winner = 'Johannes Georg Bednorz';
```
![image](https://user-images.githubusercontent.com/81769242/221490532-f9c726c3-62b3-47fe-98a8-52a581b37fd0.png)


# Task 23
```sql
SELECT * FROM nobel_win
WHERE subject NOT LIKE 'P%'
ORDER BY year DESC, winner;
```
![image](https://user-images.githubusercontent.com/81769242/221490671-54147551-be5d-4955-96c9-8ff356db8b1a.png)


# Task 24
```sql
SELECT *
FROM nobel_win
WHERE year=1970 
ORDER BY
 CASE
    WHEN subject IN ('Economics','Chemistry') THEN 1
    ELSE 0
 END ASC,
 subject,
 winner;
```
![image](https://user-images.githubusercontent.com/81769242/221490998-8b9fcba7-da8d-4cea-b90a-ddae3b786bba.png)


# Task 25
```sql
SELECT * FROM item_mast
WHERE pro_price BETWEEN 200 AND 600;
```
![image](https://user-images.githubusercontent.com/81769242/221491150-899ebb4f-6500-4675-975d-bb5bbf7a076e.png)


# Task 26
```sql
SELECT AVG(pro_price) FROM item_mast WHERE pro_com=16;
```
![image](https://user-images.githubusercontent.com/81769242/221491259-8768c548-63ae-4e8d-b6f6-b4d2ad51d219.png)


# Task 27
```sql
SELECT
  pro_name as "Item Name",
   pro_price AS "Price in Rs."
FROM item_mast;
```
![image](https://user-images.githubusercontent.com/81769242/221491346-e93fdf3e-3e27-4c86-93a9-c815bae9f3ab.png)


# Task 28
```sql
SELECT pro_name, pro_price FROM item_mast
WHERE pro_price >= 250ORDER BY pro_price DESC, pro_name;
```
![image](https://user-images.githubusercontent.com/81769242/221491688-3300a0c1-e626-4f8f-ae6c-bea6ec80f385.png)


# Task 29
```sql
SELECT AVG(pro_price), pro_com FROM item_mast
GROUP BY pro_com;
```
![image](https://user-images.githubusercontent.com/81769242/221491832-f9048463-469c-4cfd-afbb-e370060e81ac.png)


# Task 30
```sql
SELECT pro_name, pro_price FROM item_mast
WHERE pro_price = (SELECT MIN(pro_price) FROM item_mast);
```
![image](https://user-images.githubusercontent.com/81769242/221491967-9322e7ca-a5d1-4e5e-8c4b-5569a4111f0d.png)


# Task 31
```sql
SELECT DISTINCT emp_lname FROM emp_details;
```
![image](https://user-images.githubusercontent.com/81769242/221492100-b144f02d-8d96-4761-bc7e-fd88188ce5e7.png)


# Task 32
```sql
SELECT * FROM emp_details WHERE emp_lname= 'Snares';
```
![image](https://user-images.githubusercontent.com/81769242/221492366-86d1966c-8481-42f4-a951-3ccfb56b02de.png)


# Task 33
```sql
SELECT * FROM emp_details WHERE emp_dept= 57;
```
![image](https://user-images.githubusercontent.com/81769242/221492516-9b15a406-a846-4dda-9629-a52150e31cda.png)


