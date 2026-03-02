# SQLBolt --- Exercise 12 Tasks (With Solutions)

## 1. Find the number of movies each director has directed

**Query:**

``` sql
SELECT director, COUNT(*) AS movie_count
FROM movies
GROUP BY director;
```

------------------------------------------------------------------------

## 2. Find the total domestic and international sales that can be attributed to each director

**Query:**

``` sql
SELECT m.director,
       SUM(b.domestic_sales) AS total_domestic_sales,
       SUM(b.international_sales) AS total_international_sales
FROM movies AS m
JOIN boxoffice AS b
ON m.id = b.movie_id
GROUP BY m.director;
```

------------------------------------------------------------------------

*Source: SQLBolt Practice Exercises*
