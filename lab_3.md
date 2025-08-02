# Lab 3 | SQL - Joins

## 🧾 Introduction
In this lab, you’ll combine everything you’ve learned: `SELECT`, filtering with `WHERE`, ordering, limiting, aggregating with `GROUP BY`, and joining data from multiple tables using `INNER JOIN` and `LEFT JOIN`.

# 🔍 Challenge Questions

Assume that any `ID` columns are incremental, meaning that higher IDs always occurred after lower ones. For example, a customer with a higher `CustomerID` joined the bank after one with a lower `CustomerID`.

---

### 🍋 1. From the `Cards` table, get the `CardID`, `CustomerID`, and `Customer Name` of the first 5 cards.

Expected Output:
```
1	3	Heather Harris
2	3	Heather Harris
3	5	Larry Barr
4	6	Daniel Garcia
5	6	Daniel Garcia
```


### 🍋 2. List the last 5 transactions from the `CardTransactions` table along with the card `Type`. Show `TransactionID`, `Date`, and `Type`.

Expected Output:
```
673	2024-01-11	Debit
672	2022-06-30	Debit
671	2024-07-02	Debit
670	2024-05-30	Debit
669	2023-12-06	Debit
```


### 🍋 3. Show  `LoanID`s with the corresponding `Customer Name` and `LoanAmount`. List the top 5 loans by `LoanAmount` descending.

Expected Output:
```
37	Melissa Owen	        99003.41
52	Kellie Carey	        98891.75
24	Adriana Pacheco	        95903.89
20	Lisa Aguirre	        93100.54
40	Mrs. Samantha Johnson	92151.65
```


### 🍋 4. Count the customers who have never been issued a card.

Expected Output:
```
47
```


### 🌶️ 5. Show all customers along with the number of cards they hold. Include customers with 0 cards. Sort by count descending.

Expected Output:
```
Brandon Romero	2
Adriana Pacheco	2
Heather Harris	2
Andrew Perkins	2
Wayne Tucker	2
Daniel Garcia	2
...
```


### 🌶️ 6. For each customer, show the number of loans and their total loan amount. Include only customers with loans. Sort by total amount descending.

Expected Output:
```
Melissa Owen	1	99003.41
Kellie Carey	1	98891.75
Adriana Pacheco	1	95903.89
...
```


### 🌶️ 7. Show the top 5 customers who have the highest number of fraud card transactions. Include their `Name`, number of frauds as `fraud_count`, and total amount as `fraud_total`.

Expected Output:
```
Mariah Chapman	8	4431.97
Allison Summers	6	3564.59
Rebecca Frost	6	2730.55
Jessica Tran	6	2749.65
Larry West	5	2738.96
```


### 🌶️ 8. Find all customers that have never been involved in any loan.

Expected Output:
```
Heather Harris
Randy Stevens
Daniel Garcia
...
```


### 🌶️🌶️🌶️ 9. Show the top 3 accounts with the highest total incoming transaction amount (only Deposit and Transfer). Show `AccountID`, `Customer Name`, and `incoming_total`

Expected Output:
```
62	Michael Smith	46419.92
162	Rebecca Hill	46400.35
182	Heather Brennan	44748.02
```

### 🌶️🌶️🌶️ 10. For each region, find the average number of cards issued per customer. Include regions even if no cards exist.

Expected Output:
```
Alabama	        0.6667
Alaska	        1.0000
Arizona	        0.6667
Arkansas	1.0000
California	1.0000
Florida	        0.8000
Hawaii	        1.0000
Idaho	        0.3333
Illinois	0.5000
Indiana	        0.8571
Iowa	        1.0000
Kansas	        0.0000
Kentucky	0.6667
Maine	        1.0000
Maryland	0.6667
Massachusetts	1.0000
Michigan	1.0000
Minnesota	1.0000
Missouri	0.8333
Nebraska	0.0000
Nevada	        1.0000
New Hampshire	1.0000
New Jersey	0.5000
New Mexico	0.5000
New York	0.5000
North Carolina	1.0000
North Dakota	0.6667
Ohio	        1.0000
Oklahoma	0.8333
Oregon	        0.7500
Pennsylvania	0.8333
Rhode Island	0.5000
South Carolina	1.0000
South Dakota	1.0000
Texas	        0.5000
Utah	        1.0000
Vermont	        0.5000
Virginia	0.6667
Washington	0.0000
West Virginia	1.0000
Wisconsin	0.5000
Wyoming	        1.0000
```