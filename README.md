# Crime-GEO-Application
GEO Application for crime mapping and spatial queries.

Dozens of crimes are taking place these days and  mapping a crime is probably the best approach to visualize and analyze crime data.
It is a key component which allows police officers and criminalysts identify patterns in crimes:
- Hot Spots
- Spatial Behaviour 

Having a crime mapping application allows to take right actions and prevent future crimes.

The application is written on R language and uses the following main libraries:
-	Leaflet 
-	Shiny
-	DBI and RPostgreSQL

# Database description
The application uses PostgreSQL and PostGIS extension for spatial queries. Before inserting the data into the database, all tables and PostGIS extension have to be created.
