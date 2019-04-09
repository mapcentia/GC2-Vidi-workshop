# Introduction to GC2/Vidi

The GC2/Vidi framework helps you build a spatial data infrastructure quickly and easily. Powered using open source components for a scalable solution focused on freedom rather than fees.   

GC2/Vidi comprises two software projects:
- GC2 – makes it easy to deploy PostGIS, MapServer, QGIS Server, MapCache, Elasticsearch, GDAL/ogr2ogr. And offers an easy-to-use browser application to configure the software stack.   
- Vidi – a modern take on browser GIS. It is the front-end client for GC2.

This workshop will take you through the basics of using the software. You'll learn how to import vector and raster files into PostGIS, setup MapServer and QGIS server for displaying map layers in the browser GIS Vidi.

## Data for use in workshop
For this workshop we've compiled some data you can use in the exercises: [Download zip-file](https://github.com/mapcentia/GC2-Vidi-workshop/raw/master/Data.zip)

Of course you can use any data you may want. You need to know which EPSG code the projection of the data has and unless you're using ESRI Shape files, you'll need to know the geometry type of the data.

Info on the files in the package:

Vector files:   
Windmill.gml (point)  
Train_station.gml (point)  
Railroad.gml (linestring)  
City_center.gml (polygon)
municipality.zip (ESRI Shape file)

Raster files:  
SIMRAIN_1km_6320_550.tif  
SIMRAIN_1km_6320_551.tif
