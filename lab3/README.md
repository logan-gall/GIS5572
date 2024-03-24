# Lab 3: Mapping Minnesota's Terrain and Climate

In this lab, we aim to construct detailed maps showcasing the temperature variations and elevation features across Minnesota. Our primary focus is on accurately predicting these spatial attributes and evaluating the fidelity of our predictions. The resulting maps and their corresponding accuracy assessments will be stored in a database, accessible through a dedicated Flask API endpoint. Users can seamlessly view and analyze these maps using ArcOnline's intuitive MapViewer interface.
The goal of this lab is to create interpolated temperature and elevation maps for the state of Minnesota and evaluate their accuracy. The resulting maps and accuracy assessments will be stored in a database and made accessible via a Flask API endpoint for viewing on ArcOnline's MapViewer.

## Diagrams


## Contents:

Exploring Spatial Analysis in Jupyter Notebooks

Elevation Interpolation (Elevation_Interpolation.ipynb):

Utilizes QAQC'd elevation data for querying and sampling.
Executes three distinct interpolation algorithms.
Conducts accuracy evaluations and stores results in the database.
Temperature Interpolation (Temperature_Interpolation.ipynb):

Gathers QAQC'd temperature data for analysis.
Implements three interpolation algorithms for temperature mapping.
Evaluates accuracy using appropriate metrics and archives results in the database.

PDF File with Video Link:

Contains a direct link to the ArcOnline MapViewer.
Presents interpolated elevation and temperature maps.
Includes layers for accuracy assessment and point differences for comprehensive analysis.

## Key Features:

Extracts elevation and temperature point data from a database.

Samples data from both datasets, obtaining training and testing point data.

Conducts exploratory interpolation to understand the data distribution.

Utilizes IDW, Kriging, and Kernel interpolation methods for spatial estimation.

Pushes interpolated results as point data back into the database.

Performs accuracy assessment, focusing on the Kriging interpolation method.

Deploys the project on Google Cloud Run, enabling access through an API link on ArcGIS Online.



