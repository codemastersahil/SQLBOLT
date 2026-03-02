# SQLBolt --- Exercise 2 Tasks (With Solutions)

## 1. Find the movie with a row id of 6

**Query:**

``` sql
SELECT * 
FROM movies
WHERE id = 6;
```

------------------------------------------------------------------------

## 2. Find the movies released between 2000 and 2010

**Query:**

``` sql
SELECT title, year
FROM movies
WHERE year BETWEEN 2000 AND 2010;
```

------------------------------------------------------------------------

## 3. Find the movies NOT released between 2000 and 2010

**Query:**

``` sql
SELECT title, year
FROM movies
WHERE year NOT BETWEEN 2000 AND 2010;
```

------------------------------------------------------------------------

## 4. Find the first 5 Pixar movies and their release year

**Query:**

``` sql
SELECT title, year
FROM movies
ORDER BY year
LIMIT 5;
```

------------------------------------------------------------------------

