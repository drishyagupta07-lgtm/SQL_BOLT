# Exercise 15 : MariaDB Queries

## Question 1:
## This database is getting too big.
## Remove all movies that were released before 2005.
```sql
DELETE FROM movies
WHERE year < 2005;
```

## Question 2:
## Andrew Stanton has left the studio.
## Remove all movies directed by him.
```sql
DELETE FROM movies
WHERE director = 'Andrew Stanton';
```