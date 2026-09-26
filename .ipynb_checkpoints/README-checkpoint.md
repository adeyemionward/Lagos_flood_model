# Lagos State Flood Risk Model 

Title: Regional Compound Flood Inundation Modeling Using Copernicus GLO-30 DEM

Objective: Delineate low-lying residential hazard zones in Lagos State exposed to tidal interfaces and fluvial overflow.

Data Sources:

ESA Copernicus GLO-30 Digital Elevation Model (30m spatial resolution).

OpenStreetMap / HydroSHEDS vector drainage networks and administrative boundaries.

Methodology:

Coordinate unification into metric space (UTM Zone 31N / EPSG:32631).

Raster mask extraction and Affine transform bounding alignment via rasterio.plot.plotting_extent.

Coastal backscatter cleaning (> -10.0m) and astronomical tidal masking (> 0.5m).

Spatial buffering (500m) and dissolved vector operations via GeoPandas.

Boolean array intersection in NumPy for compound vulnerability delineation.

Run this script to generate Lagos_Copernicus_Flood_Vulnerability.png, attach the image and code snippet to your portfolio, and proceed directly to submitting your application.
