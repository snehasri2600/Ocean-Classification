# # Machine Learning for Ocean Classifiction

The purpose of this assignment is to develop a machine learning algorithm that classifies an ocean based on the physical and chemical properties of its water. K-nearest neighbors and decision tree classifiers were used in supervised learning processes, while k-means, agglomerative, and DBSCAN clustering were used for unsupervised learning. 

Feature data was sourced from NASA's Earthdata website, where snippets of larger datasets from December 2017 were pulled and analyzed. Datasets are in netCDF form, with dimensions of latitude, longitude, and time, which were then flattened into a 2D DataFrame.

The classification dataset, with relevant mapping, is sourced from a feature layer on ArcGIS which combines two different datasets into one by The Nature Conservancy. The dataset is a shapefile with polygon and multipolygon geometries.

Once the original datasets had been merged and cleaned, the final CSV was added to this GitHub project for loading into Google Colab. Both the supervised and unsupervised learning codes reference this GitHub file directly. Additional information can be found and datasets can be downloaded in from the links listed below.

An in-depth exploration of tthe data, its findings, and scope for future research is included in the whitepaper for this project. 


# Links to data:

Classification dataset: [Marine Ecoregions and Pelagic Provinces of the World](https://data-gis.unep-wcmc.org/portal/home/item.html?id=80567b4443f4457b822f645a2f0d70cf)
**Loading this dataset involves a high runtime. The recommendation is to run this line of code, within the data cleaning Colab link, individually and avoid the "Run All" button to prevent a runtime error. 

Feature dataset: [ECCO Atmosphere Surface Temperature, Humidity, Wind, Pressure](https://podaac.jpl.nasa.gov/dataset/ECCO_L4_ATM_STATE_05DEG_MONTHLY_V4R4)

Feature dataset: [ECCO Ocean Density, Stratification, Hydrostatic Pressure](https://podaac.jpl.nasa.gov/dataset/ECCO_L4_DENS_STRAT_PRESS_05DEG_DAILY_V4R4)

**The classiication dataset was loaded into Google Colab directly from the API. Feature data subsets were added to Google Drive, then mounted into Colab for use.
