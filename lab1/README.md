# Lab 1 -- Creating a data pipeline from arcgis primitives to cloud services.

For lab 1, we worked to create an automated data pipeline from ArcGIS to cloud software. We start with creating arcGIS primitive geometries, convert it to Well Known Text, or WKT form, which then can be pushed to a Google Cloud SQL database. Next we created a Flask application that pulls that polygon data from the database and returns the geometry WKT. To be able to use this application anywhere, we tried a few methods to run the Flask application in the cloud. One way was through a Virtual Machine in Google Compute Engine, but we ran into problems deploying that to other services. The other method was to create a Google Cloud Run service, which after some effort, we were able to get working. This Cloud Run flask application could then be added into ArcGIS online, where we can view our polygon feature directly from the database.

## Folders:

There are these folders in this lab directory:

* Flask_App_Google_Cloud -- A copy of my google cloud run flask application repository. Contains code for google cloud build and run to function.

* lab1_submission -- The files that were submitted for the end of lab1

# Execution

Flask_App_Google_Cloud is designed to run as its own git repository. This can be connected to google cloud run as a new service via continuous deployment and linking the github repo. It contains a dockerfile and requirements.txt to define docker container building and execution. It also has app.py which is a Flask application that hosts a web service that connects to a google cloud SQL database.

lab1_submission contains files that were the final submission for the assignment. It has the same app.py Flask application, a geometry.csv file which shows different ways of running primitive geometry commands, a lab1part2.ipynb file which is a first section of creating a polygon primitive and pushing data to a cloud sql database, and a video_results.pdf which contains links for an overview video, this github repository, and the final polygon geometry in arcgis online.

