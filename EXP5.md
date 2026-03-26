# List all the Canadian cities and their populations 

SELECT * FROM north_american_cities
WHERE Country = 'Canada';

# List all the cities west of Chicago, ordered from west to east

SELECT CITY FROM north_american_cities
WHERE COUNTRY = 'United States'
ORDER BY Latitude DESC;

# List all the cities west of Chicago, ordered from west to east

SELECT CITY FROM north_american_cities
WHERE  LONGITUDE < -87.629798
ORDER BY LONGITUDE ASC;

# List the two largest cities in Mexico (by population) ✓

SELECT CITY FROM north_american_citIes
WHERE COUNTRY = 'Mexico'
ORDER BY POPULATION DESC LIMIT 2;

# List the third and fourth largest cities (by population) in the United States and their population


SELECT CITY, POPULATION FROM north_american_cities
WHERE COUNTRY = 'United States'
ORDER BY POPULATION DESC
LIMIT 2 OFFSET 2;