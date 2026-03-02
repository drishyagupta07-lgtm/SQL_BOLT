
# Exercise 11 : MariaDB Queries
## Table: employees



## 1. Find the number of Artists in the studio
## (without using a HAVING clause)
```sql
SELECT COUNT(*) AS number_of_artists
FROM employees
WHERE role = 'Artist';
```

## 2. Find the number of employees of each role
## in the studio
```sql
SELECT
    role,
    COUNT(*) AS number_of_employees
FROM employees
GROUP BY role;
```

## 3. Find the total number of years employed
## by all Engineers
```sql
SELECT
    SUM(years_employed) AS total_engineer_years
FROM employees
WHERE role = 'Engineer';
```