# Real Estate Data Pipeline with AWS, Airflow, Snowflake & Power BI

![redfin-diagram](https://github.com/user-attachments/assets/234cb3d2-f9ff-4930-864b-d363682586c4)

This project implements a scalable data pipeline to extract, transform, and load real estate data from Redfin into Snowflake using AWS services. The data is later visualized in Power BI to provide insights into real estate trends.

## Overview

The pipeline involves the following stages:

1. **Data Extraction**: 
   - Redfin source data is extracted using Python.
   - The raw data is loaded into AWS S3 buckets.

2. **Transformation**:
   - Python scripts are used to transform the data.
   - Transformed data is stored in a separate S3 bucket.

3. **Snowpipe**:
   - Snowpipe automatically triggers to load transformed data from S3 into Snowflake.

4. **Data Loading**:
   - Transformed data is ingested into Snowflake for further analysis and querying.

5. **Visualization**:
   - Data in Snowflake is connected to Power BI for creating visualizations and dashboards.

6. **Orchestration with Airflow**:
   - Apache Airflow, running on an EC2 instance, orchestrates the entire process, scheduling and monitoring the data pipeline.

## Architecture

The architecture includes the following components:
- **AWS S3**: Stores raw and transformed data.
- **Python**: Handles data extraction and transformation.
- **Snowflake**: Stores the final processed data for analytics.
- **Apache Airflow**: Orchestrates the ETL pipeline.
- **Power BI**: Provides visualization for data insights.

## Technologies Used

- **Python**: For extraction and transformation scripts.
- **AWS S3**: For cloud storage of raw and transformed data.
- **Apache Airflow**: For orchestrating and automating the data pipeline.
- **Snowflake**: For cloud-based data warehousing.
- **Power BI**: For data visualization.
- **AWS EC2**: For running the Airflow instance.

## Key Features

- **Automated Data Ingestion**: Redfin data is automatically ingested and stored in S3 buckets.
- **ETL Orchestration**: Airflow schedules and monitors the ETL pipeline.
- **Real-Time Loading**: Data is continuously ingested into Snowflake using Snowpipe.
- **Visualization**: Power BI connects to Snowflake for advanced analytics and dashboards.
  
  ## Visualizations through Power BI
  ### Sum of Homes Sold
   ![sum-of-homes-sold](https://github.com/user-attachments/assets/c3e0efc4-690f-4aad-aa1d-0db25e7870f9)


  ### Sum of Inventory
   ![sum-of-inventory](https://github.com/user-attachments/assets/2bed1deb-48a0-4592-b724-753790d3041d)

