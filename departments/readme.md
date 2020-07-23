# Departments in Guatemala
Here you going to find the database of every department in Guatemala in JSON and CSV formats

## Cypher Neo4j
Return all departments
> It seems that I have some null values, dont worry I will updated tomorrow.

`` MATCH (a:pais)-[:DEPARTAMENTO_GUATEMALA]->(b:Departamento) RETURN a.name AS Pais, b.name AS Departamento, b.latitude AS Latitude, b.longitude AS Longitude, b.elevation AS Elevation, b.extensionKM AS Extension_KM, b.creacion AS Creation_date ``
