# Departments in Guatemala
Here you going to find the database of every department in Guatemala in JSON and CSV formats

## Cypher Neo4j
Return all departments
> It seems that I have some null values..

`` MATCH (a:pais)-[:DEPARTAMENTO_GUATEMALA]->(b:Departamento) RETURN a.name AS Pais, b.name AS Departamento, b.latitude AS Latitude, b.longitude AS Longitude, b.elevation AS Elevation, b.extensionKM AS Extension_KM, b.creacion AS Creation_date ``

> The next query will throw all departments order by Extension:

``MATCH (a:pais)-[:DEPARTAMENTO_GUATEMALA]->(b:Departamento) RETURN a.name AS Country, b.name AS Department, b.extensionKM AS Extension_in_KM, b.elevation AS Elevation, b.creacion AS Creation_Date, b.latitude AS Latitude, b.longitude AS Longitude ORDER BY b.extensionKM``
