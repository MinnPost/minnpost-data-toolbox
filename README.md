# MinnPost Data/Toolbox

This repo contains data that MinnPost uses often in data projects.
Most of the data is specific to Minnesota.

## Data stores

Places to find data.

### Minesota

- ??

### National

- http://www.census.gov/cgi-bin/geo/shapefiles2010/main
- http://census.ire.org/

### International

- http://data.worldbank.org

## Helpful Tools

Some helpful tools for working with data:

 - PostGIS
 - TileMill
 - CSVKit ([code](https://github.com/onyxfish/csvkit), [docs](http://csvkit.readthedocs.org/en/latest/index.html))

## Working with Minnesota Data

### GIS Projections

Minnesota geospatial data often comes in the following projection.  This
information should be available with Shapefiles.

- SRID: ```26915``` (included in PostGIS)
- WKT Projection: ```
GEOGCS["GCS_North_American_1983",DATUM["D_North_American_1983",SPHEROID["GRS_1980",6378137,298.257222101]],PRIMEM["Greenwich",0],UNIT["Degree",0.017453292519943295]],PROJECTION["Transverse_Mercator"],PARAMETER["False_Easting",500000],PARAMETER["False_Northing",0],PARAMETER["Central_Meridian",-93],PARAMETER["Scale_Factor",0.9996],PARAMETER["Latitude_Of_Origin",0],UNIT["Meter",1]]
```
- OGR: ```+proj=utm +zone=15 +ellps=GRS80 +datum=NAD83 +units=m```