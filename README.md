# openweather_api_with_airflow_AWS

## Overview
In this project, I will build and automate an ETL process that can extract current weather data from open weather map API, transform the data, load the data into AWS RDS, then join with another data in RDS and load it into an S3 bucket using Apache Airflow.
I use airflow to orchestrate a parallel processing ETL pipeline on AWS EC2.
## Project Goals
1. Data Ingestion — Build a mechanism to ingest data from from different sources.
2. ETL Pileline — I am getting data in raw format, transforming this data into the proper format and join with another data source to get more info using  Apache Airflow.
3. Cloud — In this case, I will use AWS

## Services I will be using
1. Amazon S3: Amazon S3 is an object storage service that provides manufacturing scalability, data availability, security, and performance.
2. AWS IAM: This is nothing but identity and access management which enables us to manage access to AWS services and resources securely.
3. AWS RDS Postgres: use to support relational databases Postgres
4. AWS EC2: I use it to install Apache Airflow Software.
## Data Used
1. Open Weather API
2. us_city.csv

## Architecture Diagram

<img src="images/architecture_.png">

## Detail
- Use airflow to orchestrate a parallel processing ETL pipeline on AWS EC2.
- Build and automate an ETL process that can extract current weather data from open weather API, transform the data and load the data into amazon RDS Postgres. 
- Join tables in amazon RDS, then load the result back into an S3 bucket using Apache Airflow.

## Dag Process (Airflow)

<img src="images/DagProcess.png">
