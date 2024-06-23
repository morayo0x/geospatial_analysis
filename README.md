# Geospatial Data Analysis

This repository is based on Kaggle micro-course on geospatial data analysis and visualization using the *GeoPandas* library.

### GeoPandas

It is an open sourse library for manipulating geospatial data (viewed as geometric object) using Python. It makes this possible by extending the Pandas library for operations on geometric object.

> it considers only cartesian plane *objects* such as point, curve, and a polygon as valid. Hence, a three dimensional representation of the data in a cartesian plane is considered invalid or more precisely, the z-coordinate is ignored in the analysis of the spatial data

Underneath, it depends on two important library:
- shapely: used for the "analysis and manipulation of geometric objects on Cartesian plane (two-dimensional) through set-theoretic operations such as (union, intersections, complements, differences e.t.c.)"

- fiona: it is used to read a Geographic Information System (GIS) data format from a file/memory into a simple format such as a row or records, and write data from a simple format into a GIS data format. 

	> The GIS data format is endowed with a single geometric attribute (e.g. type of geometric object, coordinates, length/distance, area, bounds e.t.c) which indicates what the simple data format represents

### Shapely
The geometric objects types used in shapely are:
- point implemented by the Point class
- collection of points is implemented by the MultiPoint class

- Curve implemented by the LineString class
- collection of points is implemented by the MultiLineString class

- Surface implemented by the Polygon class
- collection of surface is implemented by the MultiPolygon class


> it is important to note that there are no smooth (or continous) curve in shapely

### Fiona

As described above, there are different GIS file format for encodinng geographical information. Examples include

- Raster format: this divides a 2D space into rectangular grid of rows and columns of cells having a specific length and width. Each cell has a stored value - representing a geometric feature of the data. It stores both discrete and continous information. Example implementation fo this file format includes but not limited to DRG, IMG, JPEG200, MrSID e.t.c.

 > this format is typically used in remote sensing imagery, weather and climate, population density, soil properties e.t.c.

- Vector format: stores discrete information about a discrete object such as a point, line or polygon. Example implementation fo this file format includes but not limited to Shapefile, GeoJson, GML, KML, MapInfo, Spatialite e.t.c.


-- -
### Sources: 
 - Kaggle Geospatial Tutorial: [https://www.kaggle.com/code/alexisbcook/your-first-map]
 - GeoPandas Website: [http://geopandas.org/]
 - Shapely Website: [https://shapely.readthedocs.io/]
 - Fiona website: [https://fiona.readthedocs.io/]
 - GIS file format: [https://en.wikipedia.org/wiki/GIS_file_format]