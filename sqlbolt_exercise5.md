# SQLBolt --- Exercise 5 Tasks (With Solutions)

## 1. List all the Canadian cities and their populations

**Query:**

``` sql
SELECT city, population
FROM north_american_cities
WHERE country = 'Canada';
```

------------------------------------------------------------------------

## 2. Order all the cities in the United States by their latitude from north to south

**Query:**

``` sql
SELECT city, latitude
FROM north_american_cities
WHERE country = 'United States'
ORDER BY latitude DESC;
```

------------------------------------------------------------------------

## 3. List all the cities west of Chicago, ordered from west to east

**Query:**

``` sql
SELECT city, longitude
FROM north_american_cities
WHERE longitude < (
    SELECT longitude
    FROM north_american_cities
    WHERE city = 'Chicago'
)
ORDER BY longitude ASC;
```

------------------------------------------------------------------------

## 4. List the two largest cities in Mexico (by population)

**Query:**

``` sql
SELECT city, population
FROM north_american_cities
WHERE country = 'Mexico'
ORDER BY population DESC
LIMIT 2;
```

------------------------------------------------------------------------

## 5. List the third and fourth largest cities (by population) in the United States and their population

**Query:**

``` sql
SELECT city, population
FROM north_american_cities
WHERE country = 'United States'
ORDER BY population DESC
LIMIT 2 OFFSET 2;
```

------------------------------------------------------------------------


