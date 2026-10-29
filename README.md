# Azure Cloud Analytics Experiments. (USN-25MCAR0148)

This repository contains the practical implementations and outputs of three Azure Cloud Analytics experiments using Azure Data Factory, Azure Synapse Analytics, and Azure Data Lake Storage.

## Experiment 1 – ADF Pipeline: On-Prem SQL to Azure Blob Storage

This experiment demonstrates the creation of an Azure Data Factory pipeline to transfer data from an on-premises SQL Server database to Azure Blob Storage. Azure Data Factory is used as a cloud-based data integration service, with a Self-hosted Integration Runtime configured to connect the on-premises SQL Server to Azure. The pipeline uses a Copy Data Activity to move the data from the SQL Server source to Azure Blob Storage and the pipeline execution is monitored to verify successful data transfer.

## Experiment 2 – Create an Azure Synapse Dedicated SQL Pool and Load Data

This experiment demonstrates the creation of an Azure Synapse Dedicated SQL Pool and loading data into the pool for analysis. Azure Synapse Analytics provides a scalable cloud-based data warehousing environment for processing and analyzing large datasets. The Dedicated SQL Pool is configured, a table is created, data is loaded into the table, and SQL queries are executed to verify the loaded data and demonstrate cloud-based data warehousing and analytics.

## Experiment 3 – Query and Analyze Structured and Unstructured Data Using Synapse

This experiment demonstrates querying and analyzing structured and unstructured data stored in Azure Data Lake Storage using Azure Synapse Analytics. Data files are uploaded to Azure Data Lake Storage and connected to the Synapse workspace, where SQL queries are used to access and analyze the stored data. The query results are verified in Synapse, demonstrating the use of Azure services for data lake analytics, data processing, and cloud-based data analysis.

## Experiment 4: Copy CSV File from On-Premises to Azure Data Lake Storage Gen2

The objective of this experiment is to transfer a CSV file from an on-premises Windows Server to Azure Data Lake Storage Gen2 using Azure Data Factory. A CSV file named `Prajwal.csv` was created in the `C:\ADF_CA` directory, and the source and destination datasets were configured using the appropriate linked services. A pipeline was created using the Copy Data activity to transfer the file to the Azure Storage container. The pipeline was validated and executed successfully, demonstrating data movement between the on-premises environment and Azure cloud storage.

## Experiment 5: Configure Integration Runtime and Linked Services

The objective of this experiment is to configure connectivity between an on-premises Windows Server and Azure services using Azure Data Factory. A Self-Hosted Integration Runtime named `integrationRuntime-148` was configured to access the on-premises environment. The file system linked service `LS_Onprem_File_148` was configured to connect to the shared folder containing the CSV file, while the Azure Data Lake Storage Gen2 linked service `LS_adls_ingest_148` was configured to connect to the destination storage account. The connections were tested successfully, establishing the connectivity required for data integration.

## Experiment 6: Verify Data Ingestion into Azure Data Lake Storage Gen2

The objective of this experiment is to verify the successful transfer of a CSV file from an on-premises Windows Server to Azure Data Lake Storage Gen2. The Azure Data Factory pipeline was executed using the configured source and destination datasets, with the destination path set to the `raw/ingest` directory in the storage container. The pipeline execution output showed a successful status, and the Azure Portal was used to verify that `Prajwal.csv` was present in the destination directory. This experiment demonstrated successful data ingestion and verification using Azure Data Factory.
