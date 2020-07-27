# Dataset of Department El Progreso and his Population

Try the next query to return all data from department and his regions:

``MATCH (a:Departamento {name:'Progreso'})-[:MUNICIPIO_DEPARTAMENTAL]->(b:Municipio) RETURN a.name AS Department, b.name AS Region, b.creacion AS Creation_Date, b.elevation AS Altitude, b.extensionKM AS Extent, b.latitude AS Latitude, b.longitude AS Longitude ``

Or if you want to return the population data:

``	MATCH (a:Departamento {name:'Progreso'})-[:MUNICIPIO_DEPARTAMENTAL]->(b:Municipio)-[:POBLACION]->(c:Poblacion) RETURN a.name AS Department, b.name AS Region, c.censo AS Population, c.year AS Date``
