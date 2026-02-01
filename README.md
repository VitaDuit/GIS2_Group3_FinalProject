## GIS2\_Group3\_FinalProject



## 15‑Minute City Analysis of Graz, Austria

This repository contains a spatial analysis of 15‑minute city conditions in Graz, Austria. The project identifies where residents can reach five essential amenities (public transport stations, supermarkets, green spaces, pharmacies, doctors) within 1,000 m walking distance and estimates how many people live in these areas. Furthermore, areas are identified, where only one kind of amenity is missing, and it is calculated, how many people gain access to a 15-minute city by adding the missing amenity.





#### Content:

The data and scripts in this repository cover:

* City boundaries of Graz
* Street network of Graz and surrounding area (buffer 1,000 m)
* Points of interest (POIs: public transport stations, supermarkets, green spaces, pharmacies, doctors) within 1,000 m of Graz:
* Population of Graz for the year 2020 (100 × 100 m grid, GHS‑POP)
* Building footprints in Graz
* Residential areas in Graz



#### Data Sources:

OpenStreetMap Contributors:

* City boundaries
* Street Network
* POIs
* Buildings
* Residential Areas

Population Data:

* Pesaresi, M., Schiavina, M., Politis, P., Freire, S., Krasnodębska, K., Uhl, J. H., Carioli, A., Corbane, C., Dijkstra, L., Florio, P., Friedrich, H. K., Gao, J., Leyk, S., Lu, L., Maffenini, L., Mari-Rivero, I., Melchiorri, M., Syrris, V., Van Den Hoek, J., \& Kemper, T. (2023). GHS-POP R2023A — GHS population grid multitemporal (1975–2030). Dataset: GHS\_POP\_E2020\_GLOBE\_R2023A\_54009\_100\_V1\_0\_R4\_C20. European Commission, Joint Research Centre. https://doi.org/10.2905/2FF68A52-5B5B-4A22-8F40-C41DA8332CFE. Available under: https://human-settlement.emergency.copernicus.eu/download.php?ds=pop



#### Requirements:

* osmnx
* geopandas
* pandas
* matplotlib
* rasterio
* numpy
* pathlib
* networkx
* scipy
* shapely
* collections
* copy
* sklearn



#### Usage:

Clone the repository to your device. 
A preprocessed file of the population grid clipped to Graz is in the "preprocessed" folder. If you wish to do the full analysis or use it for another city, download the population grid at https://human-settlement.emergency.copernicus.eu/download.php?ds=pop, save it in the base directory and adjust the POP_RAW_PATH accordingly.
Run the cells of the Jupyter Notebook (Group3\_FinalProject.ipynb) from top to bottom. In case you have not all libraries mentioned under requirements installed, use the '!pip install' command to download the missing ones. The rest of the data is provided in this repository (preprocessed population data) or downloaded automatically by executing the code (OpenStreetMap data).
