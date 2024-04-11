# AzureETLProject_reyden
Hi this is a readme for the Azure project Demo I am completing

Features include
Azure DATA LAKE GEN 2 Storage folders: (landingzone, staging, rejected)
Azure Data Factory (storage based trigger, pipeline with Databricks notebook)\
Azure Databricks ( Data cleaning and transformations, duplicate row check, date format validation, Loading of the Azure SQL database)
Azure SQL Database (Table creation, format and Products tables)
Azure Key vault (to utilize best pratices of data security and integrity. Not having our passwords hardcode into our notebooks)

Steps
1: setup directorys in azure blob storage accounts
2: create instances of Azure sql database
3: Create data bricks account & generate secretScope (#secrets/createScope)
4: Use Azure key vault to store db password, databricks secret scope and SAS token
5: Execute .sql file in SSMS (SQL Server Management Studio)
6: upload .ipynb file to databricks workspace
7: Setup Pipeline in data factory to run notebook with a storage event trigger(@triggerBody().fileName) to pass as parameter on trigger. 
8: upload file to landingzone to trigger workflow. 
