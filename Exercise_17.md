# Exercise 17
---

## 1️⃣ Add a column named `Aspect_ratio` with FLOAT data type.

```sql
ALTER TABLE movies
ADD COLUMN Aspect_ratio FLOAT;
```

---

## 2️⃣ Add a column named `Language` with TEXT data type and default value 'English'.

```sql
ALTER TABLE movies
ADD COLUMN Language TEXT DEFAULT 'English';