# Podcast Data Pipeline using Apache Airflow
This project automates the process of extracting podcast data from a XML file and loading it into a PostgreSQL database using Apache Airflow.

Overview
Data Source: XML file containing podcast information.
Tools Used: Apache Airflow, PostgreSQL.
Workflow:
Use Apache Airflow to fetch the XML file from a specified link.
Extract relevant data from the XML file.
Load the extracted data into a PostgreSQL database.
Setup
Install Apache Airflow: Follow the official installation guide to install Airflow.
Configure Airflow: Update airflow.cfg to set up the connection to PostgreSQL.
Create a PostgreSQL Database: Create a database named podcast in PostgreSQL.
Clone the Repository: git clone https://github.com/yourusername/podcast-data-pipeline.git
Install Dependencies: pip install -r requirements.txt
Run Airflow Web Server: airflow webserver --port 8080
Run Airflow Scheduler: airflow scheduler
Usage
Start the Airflow Web Server: Navigate to localhost:8080 in your browser.
Enable the DAG: Enable the podcast_data_pipeline DAG in the Airflow UI.
Trigger the DAG: Trigger the DAG manually or wait for the scheduled run.
Monitor the Execution: Check the Airflow UI for the status of the DAG and task instances.
Check the Database: Verify that the podcast data has been successfully loaded into the PostgreSQL database.
Credits
This project was created by [Your Name]. Special thanks to the Apache Airflow and PostgreSQL communities for their amazing tools and documentation.

