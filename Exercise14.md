# Exercise 14 : MariaDB Queries

## Question 1:
## The director for "A Bug's Life" is incorrect.
## Update the record so that it reflects the correct director.
```sql
UPDATE movies
SET director = 'John Lasseter'
WHERE title = 'A Bug''s Life';
``` 

## Question 2:
## The release year for "Toy Story 2" is incorrect.
## Update the record to show the correct release year.
```sql
UPDATE movies
SET year = 1999
WHERE title = 'Toy Story 2';
```


## Question 3:
## Both the title and director for "Toy Story 8" are incorrect.
## Update the record so the title is "Toy Story 3" and the director is Lee Unkrich.
```sql
UPDATE movies
SET title = 'Toy Story 3',
    director = 'Lee Unkrich'
WHERE id = 11;

```