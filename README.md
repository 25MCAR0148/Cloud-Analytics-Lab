# Azure Cloud Analytics Experiments. (USN-25MCAR0148)

This repository contains the practical implementations and outputs of three Azure Cloud Analytics experiments using Azure Data Factory, Azure Synapse Analytics, and Azure Data Lake Storage.

## Experiment 1 – ADF Pipeline: On-Prem SQL to Azure Blob Storage

This experiment demonstrates the creation of an Azure Data Factory pipeline to transfer data from an on-premises SQL Server database to Azure Blob Storage. Azure Data Factory is used as a cloud-based data integration service, with a Self-hosted Integration Runtime configured to connect the on-premises SQL Server to Azure. The pipeline uses a Copy Data Activity to move the data from the SQL Server source to Azure Blob Storage and the pipeline execution is monitored to verify successful data transfer.

## Experiment 2 – Create an Azure Synapse Dedicated SQL Pool and Load Data

This experiment demonstrates the creation of an Azure Synapse Dedicated SQL Pool and loading data into the pool for analysis. Azure Synapse Analytics provides a scalable cloud-based data warehousing environment for processing and analyzing large datasets. The Dedicated SQL Pool is configured, a table is created, data is loaded into the table, and SQL queries are executed to verify the loaded data and demonstrate cloud-based data warehousing and analytics.

## Experiment 3 – Query and Analyze Structured and Unstructured Data Using Synapse

This experiment demonstrates querying and analyzing structured and unstructured data stored in Azure Data Lake Storage using Azure Synapse Analytics. Data files are uploaded to Azure Data Lake Storage and connected to the Synapse workspace, where SQL queries are used to access and analyze the stored data. The query results are verified in Synapse, demonstrating the use of Azure services for data lake analytics, data processing, and cloud-based data analysis.
