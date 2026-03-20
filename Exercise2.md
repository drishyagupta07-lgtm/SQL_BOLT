
# Exercise 2 : MariaDB Queries
## Table: movies


## 1. Find the movie with a row id of 6
```sql
SELECT *
FROM movies
WHERE id = 6;
```


## 2. Find the movies released between the years 2000 and 2010 (inclusive)
```sql
SELECT *
FROM movies
WHERE year BETWEEN 2000 AND 2010;
```

## 3. Find the movies NOT released between the years 2000 and 2010
```sql
SELECT *
FROM movies
WHERE year NOT BETWEEN 2000 AND 2010;
```

## 4. Find the first 5 Pixar movies and their release year
## (Ordered by earliest release year)
```sql
SELECT title, year
FROM movies
ORDER BY year ASC
LIMIT 5;
```
