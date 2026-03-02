# Exercise 16 : MariaDB Queries


## Question:
## Create a new table named `Database` with the following columns:
## Name: TEXT describing the name of the database
## Version: FLOAT representing the latest version
## Download_count: INTEGER representing the number of downloads
## This table has no constraints.
```sql
CREATE TABLE Database (
    Name TEXT,
    Version FLOAT,
    Download_count INTEGER
);
```