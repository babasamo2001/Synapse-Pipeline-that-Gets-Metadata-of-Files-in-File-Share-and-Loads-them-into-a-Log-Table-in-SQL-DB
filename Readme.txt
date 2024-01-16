
 
  Project Title: Synapse Pipeline that Gets Metadata of all Files in Azure File Shares and Loads them into a log table in Azure SQL Database

A.  Source Folder Details:
	 Number of Files: 3
	 File formats: .csv and.xlsx

B.  Output Table Details:
	 Number of Table: 1

	
C.  Business requirments:
    Client (user) needed to get Metadata of all files in Azure File Shares and loads them into a log table in Azure SQL Database
	

D.  Solution Steps: 
   	 -create RBAC role assignment for the storage account container 
   	 -create RBAC role assignment for the azure key vault
   	 -create key vault secrets for sensitive connection credentials for both daata lake container and Azure SQL database 
   	 -create link service, datasets, ETL pipeline and activities
   	 -check metadata of files in source folder and write them to the log table in Azure SQL database
   	 -check the log table to confirm the pipeline runs successfully


E.  Azure Services used: 
   	 -Azure Data Lake
   	 -Azure Data Factory
   	 -Azure SQL Database
   	 -Azure Key Vault
