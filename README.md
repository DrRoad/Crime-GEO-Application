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
* Simple Text Query (Show me Crimes in Brooklyn)
* New Crime Inserting (Add a new crime with its features)
* New Area Inserting (Can add new polygon/area of a crime)
* k-NN or Nearest Neighbour (Find closest neighbours to a certain crime)
* Searching in a Radius (Can find crimes in a certain radius)
* Searching in a Certain Area/Polygon (Can find crimes in certain areas)
* Categorical Query (Cann find a crime with specific properties,like age,place or gender...)
* Cluster Linkages (Queries which is based on formulas from Clustering in Machine Learning Field):
  * UPGMA Linkage
  * Centroid Linkage
  * Complete Linkage
  * Single Linkage

# Examples 
* Searching in a Radius:
![alt text](https://github.com/vadikl/Crime-GEO-Application/blob/master/data/pics/radius_query.png)
* Searching in a Certain Area/Polygon:
All we need to do is just draw the area and crimes will be found 
![alt text](https://github.com/vadikl/Crime-GEO-Application/blob/master/data/pics/insidepolygon_query.png)
* k-NN or Nearest Neighbour:
Let's find closest crimes to a specified one
![alt text](https://github.com/vadikl/Crime-GEO-Application/blob/master/data/pics/knn_query.png)
* Cluster Linkages (Complete Linkage)
![alt text](https://github.com/vadikl/Crime-GEO-Application/blob/master/data/pics/complete_linkage.png)
