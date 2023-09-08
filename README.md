# Twitter Data Extraction and Transformation with Airflow

This project demonstrates an end-to-end data engineering workflow for extracting data from Twitter using the Twitter API, transforming the data using Python, deploying the code on Apache Airflow running on an Amazon EC2 instance, and finally saving the transformed data on Amazon S3. The project follows best practices in data engineering, ensuring data quality, reliability, and scalability.

## Project Components:

1. **Twitter Data Extraction:**
   - Utilizes the Twitter API to extract tweets from a specified Twitter account or based on search criteria.
   - Python code is used to authenticate with the Twitter API and retrieve tweets.
   - Extracted data is in JSON format.

2. **Data Transformation:**
   - Python scripts are employed to transform the raw Twitter data into a structured format suitable for analysis.
   - Data cleaning, filtering, and enrichment processes are applied as needed.
   
3. **Airflow DAG (Directed Acyclic Graph):**
   - Defines an Airflow DAG to orchestrate the data pipeline.
   - The DAG schedules and triggers tasks for data extraction and transformation.
   - Ensures data processing on a regular basis, e.g., daily or hourly.

4. **Deployment on EC2:**
   - Code is deployed and scheduled to run on an Amazon EC2 instance.
   - EC2 instance acts as the execution environment for Airflow.
   - Ensure proper security and access controls for EC2.

5. **Amazon S3 Storage:**
   - Transformed data is saved in structured formats (e.g., CSV, Parquet) in an Amazon S3 bucket.
   - Provides scalable and cost-effective storage for the processed data.

## Project Workflow:

1. Configure your Twitter Developer account and obtain API keys.
2. Create an Airflow DAG to manage the workflow.
3. Use Python scripts to:
   - Authenticate with Twitter API.
   - Extract data from Twitter.
   - Transform the data.
   - Save the transformed data on Amazon S3.
4. Schedule the Airflow DAG to run at desired intervals (e.g., daily).
5. Deploy the code and Airflow configuration on an Amazon EC2 instance.
6. Monitor and maintain the data pipeline.

## Usage:

1. Clone this repository to your local machine or an EC2 instance.
2. Configure your Twitter API credentials and Amazon S3 settings.
3. Set up Apache Airflow with the provided DAG file.
4. Deploy and run the data pipeline.

## Dependencies:

- Python
- Tweepy (for Twitter API access)
- Apache Airflow
- Boto3 (for Amazon S3 interaction)

## Contribution:

Contributions to this project are welcome! Please feel free to submit issues, suggest enhancements, or create pull requests.
