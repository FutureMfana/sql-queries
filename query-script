/*
 These list of queries tested against the famous Northwind sample database
*/


-- Querying duplicate country entries
SELECT Country
FROM (SELECT COUNT(Country) AS Appearances, Country 
      FROM Customers
      GROUP BY country
      ORDER BY COUNT(Country))
WHERE Appearances > 1;

-- Querying non-duplicates
SELECT Country
FROM (SELECT COUNT(Country) AS Appearances, Country 
      FROM Customers
      GROUP BY country
      ORDER BY COUNT(Country))
WHERE Appearances < 2;
