# Exercise 14
---

## 1️⃣ Correct the director for *A Bug's Life* (directed by John Lasseter).

```sql
UPDATE movies
SET director = 'John Lasseter'
WHERE title = 'A Bug''s Life';
```

---

## 2️⃣ Correct the release year for *Toy Story 2* (released in 1999).

```sql
UPDATE movies
SET year = 1999
WHERE title = 'Toy Story 2';
```

---

## 3️⃣ Correct both the title and director for *Toy Story 8*.

The correct title is **Toy Story 3**  
Directed by **Lee Unkrich**

```sql
UPDATE movies
SET title = 'Toy Story 3',
director = 'Lee Unkrich'
WHERE title = 'Toy Story 8';