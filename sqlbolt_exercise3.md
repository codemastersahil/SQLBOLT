# SQLBolt --- Exercise 3 Tasks (With Solutions)

## 1. Find all the Toy Story movies

**Query:**

``` sql
SELECT title, year
FROM movies
WHERE title LIKE 'Toy Story%';
```

------------------------------------------------------------------------

## 2. Find all the movies directed by John Lasseter

**Query:**

``` sql
SELECT title, director
FROM movies
WHERE director = 'John Lasseter';
```

------------------------------------------------------------------------

## 3. Find all the movies (and director) not directed by John Lasseter

**Query:**

``` sql
SELECT title, director
FROM movies
WHERE director != 'John Lasseter';
```

------------------------------------------------------------------------

## 4. Find all the WALL-\* movies

**Query:**

``` sql
SELECT title, year
FROM movies
WHERE title LIKE 'WALL-_';
```

------------------------------------------------------------------------

