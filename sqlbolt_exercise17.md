# SQLBolt --- Exercise 17 Tasks (With Solutions)

## 1. Add a column named `Aspect_ratio`

Add a column with a FLOAT data type to store the aspect ratio each movie
was released in.

**Query:**

``` sql
ALTER TABLE Movies
  ADD COLUMN Aspect_ratio FLOAT DEFAULT 2.39;
```

------------------------------------------------------------------------

## 2. Add a column named `Language`

Add a TEXT column to store the language of the movie, with the default
value set to **English**.

**Query:**

``` sql
ALTER TABLE Movies
  ADD COLUMN Language TEXT DEFAULT "English";
```

------------------------------------------------------------------------


