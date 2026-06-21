# Azure Data Factory Mini Project

## Project Overview

This project demonstrates the creation of an end-to-end data pipeline using Azure Data Factory (ADF). The pipeline reads a CSV file from Azure Blob Storage, validates the file using the Get Metadata activity, and copies the data to a new destination location within Blob Storage.

The project covers the core concepts of Azure Data Factory, including Linked Services, Datasets, Pipelines, Metadata Validation, Data Copy Operations, and IAM Role Assignments.


## Objectives

* Create and configure Azure Storage Account.
* Upload CSV data to Azure Blob Storage.
* Create Linked Services and Datasets in Azure Data Factory.
* Validate source file availability using Get Metadata activity.
* Copy data from source to destination using Copy Data activity.
* Configure IAM roles for secure access management.
* Execute and monitor the pipeline successfully.


## Architecture

Source CSV File (Azure Blob Storage)
↓
Get Metadata Activity
↓
Copy Data Activity
↓
Destination CSV File (Azure Blob Storage)


## Technologies Used

* Microsoft Azure
* Azure Data Factory (ADF)
* Azure Blob Storage
* Azure IAM (Identity and Access Management)
* CSV Dataset


## Project Components

### 1. Azure Storage Account

A storage account was created to store source and destination data files.

### 2. Blob Container

A blob container was created and the CSV file was uploaded as the source dataset.

### 3. Linked Service

A Linked Service was configured to establish connectivity between Azure Data Factory and Azure Blob Storage.

### 4. Datasets

Two datasets were created:

* DS_Input_CSV (Source Dataset)
* DS_Output_CSV (Destination Dataset)

### 5. Get Metadata Activity

The Get Metadata activity was configured to validate the existence of the source CSV file before processing.

### 6. Copy Data Activity

The Copy Data activity was used to transfer data from the source blob location to the destination blob location.

### 7. IAM Role Assignment

The following roles were assigned:

* Reader
* Data Factory Contributor

These roles provided access control and management permissions within Azure Data Factory.


## Pipeline Workflow

1. Read source CSV file from Azure Blob Storage.
2. Validate file existence using Get Metadata activity.
3. Trigger Copy Data activity upon successful validation.
4. Copy data to destination location.
5. Monitor pipeline execution and verify successful completion.


## Expected Output

* Successful pipeline execution.
* Metadata validation completed.
* CSV file copied to destination location.
* Pipeline status displayed as "Succeeded".


## Screenshots Included

| Task         | Description                          |
| ------------ | ------------------------------------ |
| Task 1       | Azure Storage Account Creation       |
| Task 2       | Blob Container Creation & CSV Upload |
| Task 3.1     | Input Dataset Configuration          |
| Task 3.2     | Get Metadata Activity Configuration  |
| Task 3.3     | Exists Property Selection            |
| Task 4       | Pipeline Design                      |
| Task 5       | Successful Pipeline Execution        |
| Task 6       | IAM Role Assignments                 |
| Mini Project | Complete End-to-End Pipeline         |


## Learning Outcomes

Through this project, I gained hands-on experience with:

* Azure Data Factory Fundamentals
* Azure Blob Storage Integration
* Linked Services and Datasets
* Pipeline Development
* Metadata Validation
* Data Movement Activities
* IAM Role Management
* Pipeline Monitoring and Debugging
