# SQLBolt --- Exercise 14 Tasks (With Solutions)

## 1. Correct the director for *A Bug's Life*

The movie was actually directed by **John Lasseter**.

**Query:**

``` sql
UPDATE movies
SET director = "John Lasseter"
WHERE id = 2;
```

------------------------------------------------------------------------

## 2. Correct the release year for *Toy Story 2*

The correct release year is **1999**.

**Query:**

``` sql
UPDATE movies
SET year = 1999
WHERE id = 3;
```

------------------------------------------------------------------------

## 3. Correct both the title and director for *Toy Story 8*

The correct details are: - Title: **Toy Story 3** - Director: **Lee
Unkrich**

**Query:**

``` sql
UPDATE movies
SET title = "Toy Story 3", director = "Lee Unkrich"
WHERE id = 11;
```

------------------------------------------------------------------------
