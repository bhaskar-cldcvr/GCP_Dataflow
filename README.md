# GCS to BIGQUERY
Automated data pipeline to post any CSV or JSON file from local to BigQuery tables via GCS

## Prerequisites
Create a Python3 environment in local system and install the following dependencies with pip:
apache-beam==2.16.0
pandas
gcsfs

## Getting Started
Run the main.py file from /PAF/cli/main.py
python3 main.py

#### Enter the user parameters promted in the CLI
1. Choose 1 for cloud platform choice as GCP
2. Choose 1 to select programming language as Python
3. Enter the ProjectID
4. Choose 1 for pipeline source as GCS
5. Choose file format (1 for CSV, 2 for JSON)
6. Type the local absolute path for the CSV or JSON file
7. Choose the destination (2 for BigQuery)
8. Enter the Dataset name (Dataset will be validated and new Dataset will be created if not found)
9. Enter BQ table name (Table name will be validated and new Table will be created if not found)
10. Enter BQ Schema path (If left blank new schema will be automatically created from the source file)
11. Enter ETL Service as Dataflow (Option 1)
12. Enter the path of the template residing in GCS. Leave blank if template does not exist.
13. Dataflow Job will be triggerd from the existing template of after creation of the new template.

