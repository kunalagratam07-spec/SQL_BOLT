# Exercise 10
---

## 1️⃣ Find the longest time that an employee has been at the studio.

```sql
SELECT MAX(years_employed) AS longest_time
FROM employees;
```

---

## 2️⃣ For each role, find the average number of years employed by employees in that role.

```sql
SELECT role,
AVG(years_employed) AS average_years
FROM employees
GROUP BY role;
```

---

## 3️⃣ Find the total number of employee years worked in each building.

```sql
SELECT building,
SUM(years_employed) AS total_years_worked
FROM employees
GROUP BY building;