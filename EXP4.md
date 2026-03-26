# Exercise 4 — Tasks
## List all directors of Pixar movies (alphabetically), without duplicates
SELECT  distinct director
from movies
ORDER BY DIRECTOR ASC;
 
 ## List the last four Pixar movies released (ordered from most recent to least) ✓

 SELECT * FROM MOVIES
ORDER BY YEAR DESC
LIMIT 4;


## List the first five Pixar movies sorted alphabetically


SELECT * FROM MOVIES
ORDER BY title ASC
LIMIT 5;


## List the next five Pixar movies sorted alphabetically

SELECT * FROM MOVIES
ORDER BY title ASC
LIMIT 5 OFFSET 5;
