# Exercise 16
---

## 1️⃣ Create the `Database` table with the following columns:

- `Name` – A string describing the name of the database  
- `Version` – A floating-point number representing the latest version  
- `Download_count` – An integer representing the number of downloads  

```sql
CREATE TABLE Database (
    Name VARCHAR(255),
    Version FLOAT,
    Download_count INT
);