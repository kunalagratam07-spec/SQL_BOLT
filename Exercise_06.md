# Exercise 6
---

## 1️⃣ Find the domestic and international sales for each movie.

```sql
SELECT m.title,
    b.domestic_sales,
    b.international_sales
FROM movies m
JOIN boxoffice b
ON m.id = b.movie_id;
```

---

## 2️⃣ Show the sales numbers for each movie that did better internationally rather than domestically.

```sql
SELECT m.title,
    b.domestic_sales,
    b.international_sales
FROM movies m
JOIN boxoffice b
ON m.id = b.movie_id
WHERE b.international_sales > b.domestic_sales;
```

---

## 3️⃣ List all the movies by their ratings in descending order.

```sql
SELECT m.title,
    b.rating
FROM movies m
JOIN boxoffice b
ON m.id = b.movie_id
ORDER BY b.rating DESC;