# Excercise

## You can work either alone or in a group of four people

# Introduction

In order to develop detailed knowledge regarding the spatial distribution of the soil resource, digital soil mapping (DSM) techniques are increasingly being employed to add value to traditional soil maps. The basic premise that underlies DSM is various soil forming factors need to be considered during the development of a soil map. In order to generate maps of these factors cost-effectively, **covariates** that are available throughout the area are used as surrogate information. Soil forming factors such as parent material, relief, and age of land surface can easily be obtained from geological maps, remote sensing data, and digital elevation models (DEM).

A further requirement in DSM is that the relationship between soil and covariates is implemented by applying empirical models. Various **machine learning** modeling techniques have been used for the digital mapping of soils. These methods include logistic regressions, artificial neural networks, and random forest, which is perhaps the most commonly employed. 

Briefly, for DSM according to SCORPAN model, there are three requirements including soil data, covariates, and machine learning.  

# Instructions

* Use Python or R to perform the project required

* Include all of the visualizations you create to complete the project

* Include all of the codes you use to complete the project


# Background

The main aim of the project is to create digital maps of soil properties in four countries of Germany, Austria, Poland, and Czechia.

**Please choose one country**

# Datasets

## Download Dataset [**HERE**](https://github.com/RuhollahTaghizadeh/ExamGeo772022)

In the [**FILE**](https://github.com/RuhollahTaghizadeh/ExamGeo772022), there are three sub-folders: Covariates, GIS, and Soil. 

* Covariates: There are 17 covariates with the format of [**Raster**](https://www.neonscience.org/resources/learning-hub/tutorials/raster-data-r) which are derived from digital elevation model [**DEM**](https://www.usgs.gov/centers/eros/science/usgs-eros-archive-digital-elevation-shuttle-radar-topography-mission-srtm-1),  [**Landsat-8**](https://www.usgs.gov/faqs/what-are-band-designations-landsat-satellites), and climatic parameters of temprature and rainfall from [**WorldClim**](https://www.worldclim.org/data/index.html). 

* GIS: There are two files with the format of [**shapefile**](https://r-graph-gallery.com/168-load-a-shape-file-into-r.html) which are boundary of regions and point locations. The datasets are obtained from [**LUCAS**](https://esdac.jrc.ec.europa.eu/projects/lucas). 


* Soil: In this folder you can find file with the format of [**csv**](https://swcarpentry.github.io/r-novice-inflammation/11-supp-read-write-csv/) which contain the soil information of clay content (Clay),  soil organic carbon (SOC), soil acidity (pH), and cation exchange capacity (CEC). The first two columns are coordinate locations x=longitude and y=latitude.

# Remark

* It is better to work with _soil.csv_ file instead of _points.shp_ because the csv does have only the information you need.

* EPSG of the region is c("+init=epsg:4326")

* For visualization, try to use _ggplot2_ package

* For machine learning part, try to use _caret_ package
