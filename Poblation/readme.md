# Database of Population in Guatemala by Department
You cand find the data of population by department using the next query

> The next query will throw population order by Department

``MATCH (a:Departamento)-[:POBLACION]->(b:Poblacion_Departamental) RETURN a.name AS Department, b.censo AS Census, b.year AS Date ORDER BY a.name``
