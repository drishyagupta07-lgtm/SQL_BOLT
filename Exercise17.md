# Exercise 17 : MariaDB Queries

## Question 1:
## Add a column named Aspect_ratio with a FLOAT data type
## to store the aspect ratio each movie was released in.
```sql
ALTER TABLE movies
ADD COLUMN Aspect_ratio FLOAT;
``` 

## Question 2:
## Add a column named Language with a TEXT data type
## to store the language the movie was released in.
## Ensure the default language is English.
```sql
ALTER TABLE movies
ADD COLUMN Language TEXT DEFAULT 'English';
```