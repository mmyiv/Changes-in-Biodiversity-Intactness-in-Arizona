# Changes in Biodiversity Intactness Index in Arizona

## Author: [Michelle Yiv](https://github.com/mmyiv)

![Arizona Landscape. Source: azsustainabilityalliance.com](https://i0.wp.com/www.azsustainabilityalliance.com/wp-content/uploads/2019/05/Arizona_Biodiversity.jpeg?resize=1170%2C777&ssl=1)

# Purpose
In 2021, areas within Phoenix county were identified with having the most increase in developed land since 2001. This urbanization has had major effects on the surrounding environment, suggesting negative impacts on biodiversity and ecosystems.

This repository contains a Python notebook that focuses on analyzing the impact of urbanization on biodiversity in the Phoenix, Arizona county subdivision. In particular, I focus on the loss of biodiversity from 2017 to 2021 using the MPAC STAC catalog Biodiversity Intactness Index.

# Repository Structure
```
changes-in-biodiversity-intactness-in-arizona
│   README.md
|   biodiversity_impact.ipynb
|   .gitignore
│
└── data 
    │   tl_2024_04_cousub.shx
    │   tl_2024_04_cousub.shp.iso.xml
    │   tl_2024_04_cousub.shp
    │   tl_2024_04_cousub.prj
    │   tl_2024_04_cousub.dbf
    │   tl_2024_04_cousub.cpg
```
# Data Access

**1.Biodiversity Intactness Index (BII) Time Series**

Biodiversity intactness index data was accessed by the [ Microsoft Planetary Computer STAC catalog](https://planetarycomputer.microsoft.com/dataset/io-biodiversity), using the `io-biodiversity`collection. This data contains terrestrial Biodiversity Intactness maps from 2017 to 2020. To read the data, packages `pystac_client` and `planetary computer` are used to access the catalog and collection.

**2. Phoenix Subdivision Shapefile** 

Phoenix shapefile was obtained from the United States [Census Bureau Tiger/Shapeline files](https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.html). County subdivision census data from 2024 was used to filter to our area of interest. To read in the data, the `GeoPandas` package was used in addition to `os` to create an absolute filepath. 

# References

Microsoft Planetary Computer, STAC Catalog. Biodiversity Intactness. [Dataset].   https://planetarycomputer.microsoft.com/dataset/io-biodiversity. Accessed 5 December 2024.

United States Census Bureau. 2024. Arizona County TIGER/Line Shapefiles. [Dataset]. United States Census Bureau. https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.html. Accessed 5 December 2024.

