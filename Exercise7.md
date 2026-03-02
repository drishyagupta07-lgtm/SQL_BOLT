
# Exercise 7 : MariaDB Queries
## Tables: buildings, employees



## 1. Find the list of all buildings that have employees
```sql
SELECT DISTINCT building
FROM employees;
```

## 2. Find the list of all buildings and their capacity
```sql
SELECT building_name, capacity
FROM buildings;
```

## 3. List all buildings and the distinct employee roles in each building
## (including empty buildings)
```sql
SELECT DISTINCT
    buildings.building_name,
    employees.role
FROM buildings
LEFT JOIN employees
    ON buildings.building_name = employees.building;
    ```