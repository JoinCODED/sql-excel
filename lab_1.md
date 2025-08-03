# Lab | SQL - Selection

## 🧾 Introduction
In this lab, you will run basic SQL queries on a simulated banking system. You’ll use only the following SQL clauses:
* `SELECT`
* `FROM`
* `WHERE`
* `ORDER BY`
* `DISTINCT`
* `LIMIT`

# 🔍 Challenge Questions

Assume that any `ID` columns are incremental, meaning that higher IDs always occurred after lower ones. For example, a customer with a higher `CustomerID` joined the bank after one with a lower `CustomerID`.

### 🍋 1. From the `Loans` table, what are the possible loan statuses?

Expected Output:
```
Closed
Defaulted
Active
```


### 🍋 2. From the `Accounts` table, what are the balances of the first 5 Accounts?

Expected Output:
```
92855.81
68831.70
39598.73
64812.74
89911.22
```


### 🍋 3. What are the unique card types (Type) in the Cards table?

Expected Output:
```
Debit
Credit
```


### 4. From the `Customers` table, what are the names of the first 5 customers who completed KYC verification?

Expected Output:
```
Daniel Garcia
Jessica Tran
David Thompson
Timothy Bennett
Matthew Howard
```


### 5. From the `Customers` table, what is the CustomerID of the latest customer from the Wisconsin region?

Expected Output:
```
61
```


### 6. From the `Loans` table, what are the 3 lowest loan amounts?

Expected Output:
```
4822.01
12783.93
13513.40
```


### 7. From the `Loans` table, which LoanID had the highest loan amount?

Expected Output:
```
37
```


### 8. What are the CardIDs issued to CustomerID = 12?

Expected Output:
```
11
```


### 9. From the `CardTransactions` table, which CardIDs had transactions at “Martinez Group”?

Expected Output:
```
47
63
74
```


### 🌶️ 10. From the `Accounts` table, which AccountIDs have a balance between 10,000 and 20,000?

Expected Output:
```
14
33
38
43
75
86
102
107
120
133
187
192
207
```


### 🌶️ 11. From the Transactions table, show the TransactionID, Date, and Amount of the 10 most recent transactions from AccountID = 5.

Expected Output:
```
54	2024-10-17	2215.78
48	2024-08-20	2047.66
53	2024-08-04	280.48
51	2024-07-20	1579.44
56	2024-06-16	2428.71
47	2024-06-11	4073.08
50	2023-08-14	4726.52
55	2023-02-21	2750.61
52	2022-08-26	4325.90
49	2022-08-03	1655.72
```


### 🌶️🌶️ 12. From the `Cards` table, what are the last 5 CustomerIDs that have the latest expired credit cards?

Expected Output:
```
98
94
80

```
