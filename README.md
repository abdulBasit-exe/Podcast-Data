# Podcast Data Pipeline using Apache Airflow
![Podcast Data Pipeline](https://github.com/abdulBasit-exe/Podcast-Data/assets/106882008/ab045e4e-a68d-425d-a172-296c150a9a7b)

This project automates the process of extracting podcast data from an XML file and loading it into a PostgreSQL database using Apache Airflow.

## Overview
### Data Source: Link containing XML code having podcast information.
### Tools Used: Apache Airflow, PostgreSQL.

## Workflow:
- Use Apache Airflow to fetch the [XML File](https://www.marketplace.org/feed/podcast/marketplace/).
- Extract relevant data from the XML file.
- Load the extracted data into a PostgreSQL database.

### Setup
- Install Apache Airflow: Follow the official installation guide to install Airflow.
- Configure Airflow: Update airflow.cfg to set up the connection to PostgreSQL.
- Create a PostgreSQL Database: Create a database named podcast in PostgreSQL.
- Install Dependencies: pip install apache-airflow-providers-postgres
- Run Airflow Web Server: `airflow webserver -p 8080`
- Run Airflow Scheduler: `airflow scheduler`

### Usage
- Start the Airflow Web Server: Navigate to localhost:8080 in your browser.
- Enable the DAG: Enable the podcast_summary DAG in the Airflow UI.
- Trigger the DAG: Trigger the DAG manually or wait for the scheduled run.
- Monitor the Execution: Check the Airflow UI for the status of the DAG and task instances.
- Check the Database: Verify that the podcast data has been successfully loaded into the PostgreSQL database.

### Monitoring Dag On Webserver 
![image](https://github.com/abdulBasit-exe/Podcast-Data/assets/106882008/092400be-40aa-42b9-ad19-32ea1d07cd68)
### Quering Data from Database Table
![image](https://github.com/abdulBasit-exe/Podcast-Data/assets/106882008/17d9e5d6-3e2c-4182-867d-653b9f3a4bd9)

