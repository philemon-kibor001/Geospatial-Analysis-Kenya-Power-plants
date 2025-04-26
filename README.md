# Geospatial-Analysis-Kenya-Power-plants
Adding data to map using python
 visualizing power plant locations in Kenya using geospatial data and libraries like geopandas, matplotlib, and folium.

Here's a breakdown:

Data Loading:

Imports necessary libraries: geopandas, matplotlib.pyplot, folium.
Attempts to load a shapefile named "KEN_PowerPlants.shp" containing power plant data. If the file is not found locally, it prompts the user to upload it.
Reads the shapefile into a GeoDataFrame called gdf using geopandas.read_file().
Basic Visualization:

Prints the first few rows and the Coordinate Reference System (CRS) of the GeoDataFrame to provide an overview of the data.
Uses gdf.plot() to create a simple plot of the power plant locations, likely as points on a map.
Interactive Mapping with Folium:

Creates a folium map centered on Kenya using folium.Map().
Iterates through the power plant data in gdf and adds markers to the map for each power plant location using folium.Marker().
Attempts to use the 'NAME' column for marker popups, falling back to 'PLANT' if 'NAME' is not found.
Adding Popups with Plant Names:

Creates another folium map similar to the previous step.
Adds markers with popups showing the plant names, assuming the plant name is in the 'PLANT' column of the GeoDataFrame.
