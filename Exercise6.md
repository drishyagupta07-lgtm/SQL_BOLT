
# Exercise 6 : MariaDB Queries
## Tables: movies, boxoffice



## 1. Find the domestic and international sales for each movie
```sql
SELECT 
    movies.title,
    boxoffice.domestic_sales,
    boxoffice.international_sales
FROM movies
JOIN boxoffice
    ON movies.id = boxoffice.movie_id;
```

## 2. Show the sales numbers for each movie that did better
## internationally rather than domestically
```sql
SELECT 
    movies.title,
    boxoffice.domestic_sales,
    boxoffice.international_sales
FROM movies
JOIN boxoffice
    ON movies.id = boxoffice.movie_id
WHERE boxoffice.international_sales > boxoffice.domestic_sales;
```

## 3. List all the movies by their ratings in descending order
```sql
SELECT 
    movies.title,
    boxoffice.rating
FROM movies
JOIN boxoffice
    ON movies.id = boxoffice.movie_id
ORDER BY boxoffice.rating DESC;
```