# Database of Population in Guatemala by Department
We have the census and the date when official release of data population.

> The next query will throw population order by Department
``MATCH (a:Departamento)-[:POBLACION]->(b:Poblacion_Departamental) RETURN a.name AS Department, b.censo AS Census, b.year AS Date ORDER BY a.name``
