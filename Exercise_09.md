# Exercise 9
---

## 1️⃣ List all movies and their combined sales in millions of dollars.

```sql
SELECT m.title,
    (b.domestic_sales + b.international_sales) / 1000000 AS total_sales_millions
FROM movies m
JOIN boxoffice b
ON m.id = b.movie_id;
```

---

## 2️⃣ List all movies and their ratings in percent.

```sql
SELECT m.title,
    b.rating * 10 AS rating_percent
FROM movies m
JOIN boxoffice b
ON m.id = b.movie_id;
```

---

## 3️⃣ List all movies that were released in even number years.

```sql
SELECT title, year
FROM movies
WHERE year % 2 = 0;