
# Exercise 9 : MariaDB Queries
## Tables: movies, boxoffice



## 1. List all movies and their combined sales
## (in millions of dollars)
```sql
SELECT
    movies.title,
    (boxoffice.domestic_sales + boxoffice.international_sales) / 1000000
        AS combined_sales_millions
FROM movies
JOIN boxoffice
    ON movies.id = boxoffice.movie_id;
```

## 2. List all movies and their ratings in percent
```sql
SELECT
    movies.title,
    boxoffice.rating * 10 AS rating_percent
FROM movies
JOIN boxoffice
    ON movies.id = boxoffice.movie_id;
```

## 3. List all movies that were released in even-numbered years
```sql
SELECT *
FROM movies
WHERE year % 2 = 0;
```