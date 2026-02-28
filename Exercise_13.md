# Exercise 13
---

## 1️⃣ Add the studio's new production, Toy Story 4 to the list of movies.

```sql
INSERT INTO movies (id, title, director, year, length_minutes)
VALUES (15, 'Toy Story 4', 'John Lasseter', 2019, 100);
```
---

## 2️⃣ Add Toy Story 4 to the BoxOffice table.

```sql
INSERT INTO boxoffice (movie_id, rating, domestic_sales, international_sales)
VALUES (15, 8.7, 340000000, 270000000);