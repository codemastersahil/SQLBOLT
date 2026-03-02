# SQLBolt --- Exercise 7 Tasks (With Solutions)

## 1. Find the list of all buildings that have employees

**Query:**

``` sql
SELECT DISTINCT building
FROM employees;
```

------------------------------------------------------------------------

## 2. Find the list of all buildings and their capacity

**Query:**

``` sql
SELECT * FROM buildings;
```

------------------------------------------------------------------------

## 3. List all buildings and the distinct employee roles in each building (including empty buildings)

**Query:**

``` sql
SELECT DISTINCT building_name, role 
FROM buildings 
  LEFT JOIN employees
    ON building_name = building;
```

------------------------------------------------------------------------


