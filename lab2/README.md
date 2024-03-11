# Lab 2 -- Adding QAQC to our data pipelines.

For our GIS 5572 Lab 2 project, we focused on implementing QAQC to our class final projects. To do this, we downloaded five sets of data, and then designed and created multiple quality checks for each data source. We downloaded NLCD Landcover data, Minnesota elevation, and daily temperature based on lab requirements. We also generated a large event list and road traffic lines based on our final project to predict traffic conditions near the University of Minnesota.

The QAQC expands on our overall data pipeline. When working on large projects, we need to ensure that high quality products are being created. If the input data is poor, then the downstream products will also be poor. So, for each of our data sources, we performed QAQC checks. If no errors were found, we allowed data to be pushed to a cloud database. If errors were identified, we performed data reviews, leading us to make edits to the download process or remove bad points before double checking and pushing to our database.

## Folders:

There is one folder in this lab directory:

* lab2_submission -- The files that were submitted for the end of lab2

* lab2_submission/Diagrams -- Diagrams for Data flow and QAQC for this lab.

# Execution

lab2_submission contains files that were the final submission for the assignment. It has a  five .ipynb Jupyter notebooks, and a video_results.pdf which contains links for an overview video and this github repository. The five files are expected to run in an ArGIS notebooks environment. The file paths are defined relatively at the start of the file, but it is generally expected that data is downloaded to the project root folder in ArcGIS Pro. Each .ipynb file has different package requirements. A list of the five files and their description:

* Landcover -- Data flow to download NLCD landcover data from the Minnesota Geospatial Commons, and then perform QAQC checks.

* Elevation -- Data flow to download Elevation data from the Minnesota Geospatial Commons, and then perform QAQC checks.

* Temperature -- Data flow to download temperature data from the NOAA web2 API, and then perform QAQC checks.

* Sporting Events -- Data flow to download sporting event data from UMN's Gopher Sports text repository.

* Traffic Lines -- Data flow to generate baseline and large event service area analysis layers, and then perform QAQC checks.


## Attributions

Author: Logan Gall, gall0487

Attributions/Assistance:
Laure Briol,
Gregory Kohler,
ESRI Arcpy documentation,
ChatGPT,
LucidChart