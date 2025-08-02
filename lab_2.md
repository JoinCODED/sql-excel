# Lab | SQL - Aggregation

## 🧾 Introduction
In this lab, we are adding the `GROUP BY` clause and aggregation functions like `COUNT`, `SUM`, and `AVG` to our SQL vocabulary.

# 🔍 Challenge Questions

Assume that any `ID` columns are incremental, meaning that higher IDs always occurred after lower ones. For example, a customer with a higher `CustomerID` joined the bank after one with a lower `CustomerID`.

---

### 1. From the `Customers` table, how many customers are from each region? Sort by region name alphabetically.

Expected Output:
```
Alabama			2
Alaska			1
Arizona			2
Arkansas		3
California		3
Florida			3
Hawaii			3
Idaho			3
Illinois		2
Indiana			5
Iowa			1
Kansas			1
Kentucky		2
Maine			2
Maryland		3
Massachusetts	        2
Michigan		2
Minnesota		2
Missouri		4
Nebraska		1
Nevada			4
New Hampshire	        1
New Jersey		2
New Mexico		3
New York		2
North Carolina	        2
North Dakota	        2
Ohio			1
Oklahoma		4
Oregon			3
Pennsylvania	        4
Rhode Island	        2
South Carolina	        1
South Dakota	        1
Texas			3
Utah			4
Vermont			3
Virginia		3
Washington		1
West Virginia	        3
Wisconsin		3
Wyoming			1
```

---

### 2. From the `Cards` table, how many cards exist for each `Type`? Rank the results starting with the most frequent type.

Expected Output:
```
Debit	64
Credit	42
```

---

### 3. Using the `Loans` table, print the top 10 `CustomerID`s based on the sum of all of their loan amounts.

Expected Output:
```
68
97
37
29
77
82
27
93
43
56
```

---

### 4. From the `CardTransactions` table, retrieve the number of transactions issued for each `Date` after `2024-12-01`, ordered by date in descending order.

Expected Output:
```
2024-12-31	1
2024-12-29	1
2024-12-26	1
2024-12-24	1
2024-12-22	2
2024-12-20	1
2024-12-19	1
2024-12-13	1
2024-12-09	4
2024-12-07	1
2024-12-06	1
2024-12-05	1
2024-12-04	1
```

---

### 5. From the `Loans` table, how many loans were issued for each `LoanType`?

Expected Output:
```
Auto		23
Personal	16
Home		14
```

---

### 6. From the `Transactions` table, for `AccountID = 5`, show the total amount per transaction `Type`. Include `AccountID`, `Type`, and total `Amount`, sorted alphabetically by `Type`.

Expected Output:
```
5	Deposit		3235.16
5	Transfer	13444.09
5	Withdrawal	9404.65
```

---

### 7. From the `Transactions` table, calculate the average transaction amount for each `Type`, sorted by highest to lowest average.

Expected Output:
```
Transfer	2557.182244
Deposit		2499.168080
Withdrawal	2485.750690
```
