# AWS End to End Data Warehouse Implementation

## Project Overview

This project demonstrates a cloud-based Data Warehouse implementation using AWS services to collect, process, and analyze COVID-19 data. The workflow includes data ingestion, ETL, modeling, and visualization for real-time insights.

### Tech Stack

✅ Cloud Services: AWS S3, AWS Glue, AWS Athena, AWS Redshift\
✅ Data Processing: Python (Pandas, Boto3), SQL\
✅ ETL Workflow: Data ingestion, cleaning, transformation\
✅ Visualization: Dashboards using Redshift queries

## Project Architecture

🔹 Data Sources: COVID-19 case data from https://dj2taa9i652rf.cloudfront.net \
🔹 Storage: AWS S3 for raw data, AWS Redshift for structured storage\
🔹 Processing: AWS Glue for ETL transformations\
🔹 Querying: AWS Athena for quick access to processed data\
🔹 Visualization: Redshift queries to analyze COVID-19 trends

## Step-by-Step Implementation

### 1️⃣ Data Ingestion & Storage
Extract COVID-19 case data & hospital recordx.
Store raw datasets into AWS S3 buckets.
Use AWS Glue Crawlers to generate schemas automatically.
### 2️⃣ Data Transformation & Cleaning
Use Python & Pandas to clean and preprocess data.
Handle missing values & incorrect schema mappings.
Convert relational data model into Star Schema for reporting.
### 3️⃣ Data Querying & Optimization
Use AWS Athena to query raw data from S3.
Optimize queries by creating partitioned tables.
### 4️⃣ Loading Data into Redshift
Create relational tables in Amazon Redshift.
Use the COPY command to load cleaned data from S3 to Redshift.
Perform query performance tuning using indexing & partitioning.
### 5️⃣ Visualization & Reporting
Execute SQL queries in Redshift to generate insights.
Analyze case trends, hospitalizations, and regional spread.
