
# Exercise 12 : MariaDB Queries
## Tables: movies, boxoffice


## 1. Find the number of movies each director has directed
```sql
SELECT
    director,
    COUNT(*) AS number_of_movies
FROM movies
GROUP BY director;
```

## 2. Find the total domestic and international sales
## that can be attributed to each director
```sql
SELECT
    movies.director,
    SUM(boxoffice.domestic_sales) AS total_domestic_sales,
    SUM(boxoffice.international_sales) AS total_international_sales
FROM movies
JOIN boxoffice
    ON movies.id = boxoffice.movie_id
GROUP BY movies.director;
```