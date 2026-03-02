
# Exercise 13 : MariaDB Queries

## Question 1:
## Add the studio's new production, "Toy Story 4", to the movies table.
## (Any director may be used.)
```sql
INSERT INTO movies (id, title, director, year, length_minutes)
VALUES (15, 'Toy Story 4', 'Josh Cooley', 2019, 100);
``` 

## Question 2:
## "Toy Story 4" received critical acclaim.
## It has a rating of 8.7, earned 340 million domestically,
## and 270 million internationally.
## Add this information to the boxoffice table.
```sql
INSERT INTO boxoffice (movie_id, rating, domestic_sales, international_sales)
VALUES (15, 8.7, 340000000, 270000000);
```
