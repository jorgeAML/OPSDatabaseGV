# Data of every area in this department and his population

Try to get the query and his dataset using the next query in Neo4j:

``MATCH (a:Departamento {name:'Guatemala'})-[:MUNICIPIO_DEL_DEPARTAMENTO_DE_GUATEMALA]->(b:Municipio) RETURN a.name AS Department, b.name AS Municipio, b.latitude AS Latitude, b.longitude AS Longitude, b.elevation AS Altitude, b.extensionKM AS Extent ORDER BY b.name ``

If you need to extract the population by Region, try the next query:

`` MATCH (a:Municipio)-[:POBLACION]->(b:Poblacion) RETURN a.name AS Region, b.censo AS Population, b.year AS Date ``
