# Land Cover - Cantabria

This repository contains the land cover classification of the **Cantabria region (Spain)**, based on **Sentinel-2 imagery from 2021 to 2024**. The data have been processed and reprojected for geospatial analysis and area calculation in metric units.

---

## Repository Contents

- `cantabria-S2_2021_LC_UTM32630_meta.tif`  
  Raster reprojected to **EPSG:32630 (WGS84 / UTM zone 30N)** with added metadata:
  - Reference date: 2021  
  - Description: Classified land cover image  
  - Resolution: pixel size in meters  
  - Coordinate system: EPSG:32630  
  - Region: Cantabria  

- `2021/cantabria-S2_2021_LC_UTM32630.shp`  
  Shapefile generated from the raster, containing the following fields:
  - `id`: Unique identifier  
  - `Clase_lc`: Land cover class name (Pasture, Shrubland, Forest, Others)  
  - `Codigo_lc`: Numeric code associated with the class  
  - `Superficie_m2`: Polygon area in square meters  
  - `Superficie_ha`: Polygon area in hectares  
  - `Fecha_ref`: Reference year of the image  
  - `geometry`: Polygon geometry

---

## Land Cover Classes

| Code | Class       |
|------|------------|
| 1    | Pasture     |
| 2    | Shrubland   |
| 3    | Forest      |
| 4    | Others      |

---

## Usage

1. Open the TIFF or SHP files in **QGIS** or any compatible GIS software.  
2. The raster can be used for land cover analysis and area calculations.  
3. The shapefile allows vector analysis, statistics, and export to other formats.

