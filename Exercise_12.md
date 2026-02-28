# Exercise 12
---

## 1️⃣ Find the number of movies each director has directed.

```sql
SELECT director,
COUNT(*) AS number_of_movies
FROM movies
GROUP BY director;
```

---

## 2️⃣ Find the total domestic and international sales that can be attributed to each director.

```sql
SELECT m.director,
SUM(b.domestic_sales + b.international_sales) AS total_sales
FROM movies m
JOIN boxoffice b
ON m.id = b.movie_id
GROUP BY m.director;