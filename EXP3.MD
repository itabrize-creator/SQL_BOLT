*Question 1:-* Find all the Toy Story movies
```sql
SELECT *
FROM Movies
WHERE Title LIKE 'Toy Story%';
```

*Question 2:-* Find all the movies directed by John Lasseter
```sql
SELECT *
FROM Movies
WHERE Director = 'John Lasseter';
```

*Question 3:-* Find all the movies (and director) not directed by John Lasseter
```sql
SELECT title, director FROM movies
WHERE director NOT LIKE 'John Lasseter';
```

*Question 4:-* Find all the WALL-* movies
```sql
SELECT *
FROM Movies
WHERE Title LIKE 'WALL-%';
```