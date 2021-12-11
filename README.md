# CadorsMap.ca
Aviation Safety in Canada: Facts and Predictions.

## Frontend URL: www.cadorsmap.ca

Account name: `cadorsquicksightuser`

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

*More detailed instructions are available in the file* 'RUNNING.txt`


## Technologies Used
* Python and PySpark
* Selenium and Beautiful Soup for scraping
* AWS S3, Lambda, SQS, Glue, Athena, and Quicksight for Cloud Pipeline
* Photon, Nominatim, MeteoStat for Geocoding/weather augmentation

## High-level System Design

![image](https://user-images.githubusercontent.com/52950086/145689353-1ce43015-1e37-40f7-bb9d-1c5b6f31a9fc.png)


## ML Classification Engine: Predicting casualities 

![image](https://user-images.githubusercontent.com/52950086/145689402-c2c4de6b-3a7e-4dbb-b045-40d8c6d1d12a.png)


**Acheived 70% Test Accuracy with Logistic Regression.**


## The Final Product

![image](https://user-images.githubusercontent.com/52950086/145689258-b98d94d0-2cd3-4b87-bb28-25faf5d83fe7.png)
