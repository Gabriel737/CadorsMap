# CadorsMap.ca
Aviation Safety in Canada: Facts and Predictions.

![image](https://user-images.githubusercontent.com/52950086/145689258-b98d94d0-2cd3-4b87-bb28-25faf5d83fe7.png)

## Frontend URL: www.cadorsmap.ca

Account: `cadorsquicksightuser`

Username: `quicksight_reader`

Password: `quicksight@cadorscmpt732`

## Brief Overview
* Created a highly interactive visual dashboard to display Canadian aviation incident and accident statistics
* Scrapes new records from Transport Canada CADORs website on a weekly basis using serverless cloud technologies
* Developed an ML Classification Engine which predicted the likelihood of a casualty resulting from an incident with 70% test accuracy.
* Implemented a k-means Clustering algorithm to identify key attributes of CADORs records that resulted in casualties.

## Setup
* Use the two provided scraper applications to perform the initial processing of CADORs records and store the results in an S3 bucket
* Setup the given scripts in AWS, and connect the components as indicated on the system design graphic.
* Connect your QuickSight dashboard to Athena and publish it on an available domain.

*More detailed instructions are available in the file* `RUNNING.txt`


## Technologies Used
* Python and PySpark
* Selenium and Beautiful Soup for scraping
* AWS S3, Lambda, SQS, Glue, Athena, and Quicksight for Cloud Pipeline
* Photon, Nominatim, and MeteoStat for Geocoding and Weather Augmentation

## High-level System Design

![image](https://user-images.githubusercontent.com/52950086/145689353-1ce43015-1e37-40f7-bb9d-1c5b6f31a9fc.png)


## ML Classification Engine: Predicting casualities 

![image](https://user-images.githubusercontent.com/52950086/145692821-b6b34f64-f3f3-4d2b-b39e-56f96faadd39.png)


**Given the input features of an aviation incident, predicted whether or not fatalities would result with 70% Test Accuracy.**

### Contributors: @gabriel737, @kaumil, @gurashish, @arshahuja


