# SSIS-WhoISDB-Project
- Fetched data in the form of zip files from online WhoIs Database Samples and created a Data Integration Process in the MS SQL Server Integration Service.
- Used Visual Studio to create a Project Deployment Model which can be used as a SSIS catalogue in the SQL Server 2019.
- Designed the SSIS package in order to read and map source configuration data to a variable and download the data from the URL given below using script task in Visual Studio.

  WhoIs Database Sample Data Download Link:
  https://www.whoisxmlapi.com/whois-database-download.php

- Unzipped the source files using 7 Zip open source file archiver by linking it with the Execute Process Task in Visual Studio.
  Link to download: https://www.7-zip.org/download.html

- Created a Data Flow Task in order to connect to the SQL Server Database and insert the extracted files data into a table named DomainWhoIsInfo.
- Archived the files in order to avoid duplication using the File System Task option.
- Learnt how to use a script task to write a C# code in order to create a task which sends email notiications to respective users upon package execution status.
- Used Event Handlers to configure on error/success email notifications according to the package execution.
