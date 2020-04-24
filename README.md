# Crimes-GEO-Application
GEO Application for crime mapping and spatial queries.

![alt text](https://github.com/vadikl/Crime-GEO-Application/blob/master/data/pics/interface.png)

Dozens of crimes are taking place these days and  mapping a crime is probably the best approach to visualize and analyze crime data.
It is a key component which allows police officers and criminalysts identify patterns in crimes:
- Hot Spots
- Spatial Behaviour 

Having a crime mapping application allows to take right actions and prevent future crimes.

# Application Tools 
The application is written on R language and uses the following main libraries:
-	Leaflet 
-	Shiny
-	DBI and RPostgreSQL

# Dataset Description
The first dataset contains crime data and can be easily downloaded from the website of New York City:
* NYC Open Data: https://opendata.cityofnewyork.us/

The second dataset contains boroughs of New York:
* ArcGIS Hub: https://hub.arcgis.com/datasets/DCP::new-york-city-borough-boundary-clipped-to-shoreline

![alt text](https://github.com/vadikl/Crime-GEO-Application/blob/master/data/pics/city.png)
![alt text](https://github.com/vadikl/Crime-GEO-Application/blob/master/data/pics/data_set.png)

# Database description
The application uses PostgreSQL and PostGIS extension for spatial queries. Before inserting the data into the database, all tables and PostGIS extension have to be created.

![alt text](https://github.com/vadikl/Crime-GEO-Application/blob/master/data/pics/db_structure.png)

# Implemented Spatial Queries 

