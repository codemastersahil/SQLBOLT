# SQLBolt --- Exercise 10 Tasks (With Solutions)

## 1. Find the longest time that an employee has been at the studio

**Query:**

``` sql
SELECT MAX(years_employed) as Max_years_employed
FROM employees;
```

------------------------------------------------------------------------

## 2. For each role, find the average number of years employed by employees in that role

**Query:**

``` sql
SELECT role, AVG(years_employed) as Average_years_employed
FROM employees
GROUP BY role;
```

------------------------------------------------------------------------

## 3. Find the total number of employee years worked in each building

**Query:**

``` sql
SELECT building, SUM(years_employed) as Total_years_employed
FROM employees
GROUP BY building;
```

------------------------------------------------------------------------

