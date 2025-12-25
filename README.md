# credi_card_transaction_ETL_GCP_project
GCP Credit card transcation project using tech stack -  GCS, Cloud Composer, Pyspark, BigQuery, GitHubAction


<img width="1080" height="563" alt="image" src="https://github.com/user-attachments/assets/aeb38740-be4c-4f64-95d0-542980c7a7e0" />

This project demonstrates a production-ready, end-to-end credit card transaction processing pipeline built on Google Cloud Platform. 
Raw transaction JSON files arriving in Google Cloud Storage are automatically detected and orchestrated by Apache Airflow, 
which triggers a serverless PySpark job on Dataproc. 

The Spark job validates and enriches transaction data, categorizes transactions, detects high-risk and potentially fraudulent activity,
updates customer reward points, and stores the final analytics-ready data in BigQuery. Processed files are safely archived to prevent reprocessing. 
The project follows enterprise best practices by including unit tests with PyTest to validate business logic 
and a CI/CD pipeline to automatically run tests and enforce code quality on every change.

Project Execution Steps (High Level)

1. Transaction File Arrival

2. GCS File Detection via Airflow

3. Automatic Pipeline Trigger

4. Dataproc Serverless Job Execution

5. Data Validation

6. Business Transformations

7. Data Enrichment

8. Load to BigQuery

9. Archive Processed Files

10. Testing and CI/CD Quality Checks
