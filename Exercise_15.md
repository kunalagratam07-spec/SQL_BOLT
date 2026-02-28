# Exercise 15
---

## 1️⃣ Remove all movies that were released before 2005.

```sql
DELETE FROM movies
WHERE year < 2005;
```

---

## 2️⃣ Remove all movies directed by Andrew Stanton.

```sql
DELETE FROM movies
WHERE director = 'Andrew Stanton';