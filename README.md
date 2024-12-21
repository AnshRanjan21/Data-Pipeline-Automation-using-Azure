# Online Retail Store Data Pipeline Automation

This repository showcases an end-to-end data engineering project where data from an online retail store is processed and analyzed using Azure services. The project demonstrates the use of modern data engineering practices, including ETL pipelines, data lake management, and CI/CD implementation.

## Project Overview

### Objectives
- Ingest data into Azure Data Lake.
- Organize data into Bronze, Silver, and Gold layers.
- Perform ETL processes and business logic using Azure Databricks.
- Automate data processing pipelines using Azure Data Factory.
- Manage version control and implement CI/CD pipelines using Azure DevOps.

## Project Architecture

### 1. Data Ingestion
- **Source:** Online retail store data.
- **Destination:** Azure Data Lake (Bronze layer container).

### 2. Data Transformation
- **Azure Databricks Workspace**
  - Silver Layer Notebook: ETL processes to clean and transform data.
  - Gold Layer Notebook: Business logic for analysis and reporting.

### 3. Automation
- Azure Data Factory pipelines are used to automate the execution of the notebooks in sequence, based on success conditions.

### 4. Data Storage
- Transformed data is stored in Azure Data Lake containers in Parquet format for efficient querying.

### 5. Version Control and CI/CD
- **Azure DevOps Repositories**
  - Branches: Development, Main, and Production.
  - Changes pushed to the main branch trigger a CI/CD pipeline.
- **CI/CD Pipeline**
  - Automatically syncs changes from the main branch to the production branch.
  - Deploys the latest code to a release folder in the Azure Databricks workspace.

## Tools and Technologies
- **Azure Services:** Data Lake, Data Factory, Databricks
- **File Format:** Parquet
- **Version Control:** Azure DevOps Repositories
- **CI/CD:** Azure DevOps Pipelines
