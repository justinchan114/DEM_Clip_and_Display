# DEM_Clip_and_Display
Digital Elevation Model(DEM) clipping and crs projection with GDAL, and display with folium.

## Area of study
The area of study is in Abbotsford, BC, Canada.

## Raw data
LiDAR collection was obtained from Province of British Columbia, Canada, at https://www2.gov.bc.ca/gov/content/data/geographic-data-services/lidarbc. The LiDAR set obtained has a BCGS Tile Name: 092g010, and Grid Scale of 1:20000, with CRS of EPSG:3157. Downloaded here: https://nrs.objectstore.gov.bc.ca/gdwuts/092/092g/2016/dem/bc_092g010_xl1m_utm10_170713.tif

## Clipping of DEM and displaying in folium
A area was defined in a shape file in QGIS, and it is used to define the boundary of clipping with gdal.Warp. 
The data are then processed with followings:-
1. Read as numpy array 
2. Projected to EPSG:4326
3. Normalized and colorized for display in folium
4. Displayed in folium along with legend
