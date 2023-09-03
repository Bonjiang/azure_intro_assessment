
# Storage

### *Azure Backup*

#### About the Service

This service protects data and against ransomware, providing data recovery and backup with ease from Microsoft Azure cloud. It offers many benefits, such as unlimited data transfer, offload on-premises backup, automatic storage management, long-term and short-term data retention, and multiple storage options. To protect against ransomware, Azure Backup offers security both when data is in transit and at rest while using enhanced features to provide high levels of security to backed-up data. 

#### Python Integration

You can leverage Azure SDK to interact with the Azure Backup Service using Python.  

Recovery Services Backup Management Library **‘azure-mgmt-recoveryservicesbackup'**  

‘azure-identity’ library also has to be installed and authentication has to occur.  

You can list and manage backup items, and trigger and restore operations if needed.  

### *Azure Data Share*  

#### About the Service

The service provides data-sharing with third-party organizations in a safe and secure way. It simplifies the management and tracking of shared data, so users can track who shared and when. With this service, data-sharing and management is conducted in one place. Sharing frequency and access can be modified and third parties can combine data at ease. 

#### Python Integration

You can leverage Azure SDK to interact with the Azure Data Share service using Python. 

Microsoft Azure Datashare Management Client Library **‘azure-mgmt-datashare’** 

Browse code samples for [Data Share Management](https://learn.microsoft.com/en-us/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing)

# Compute

### *App Service*

#### About the Service

This HTTP-based service allows users to build and host web applications, mobile back ends, and RESTful APIs in the preferred programming language without infrastructure management. It supports various environments and there are many key features, such as multiple languages and frameworks, DevOps optimization, authentication, Visual Studio and Visual Studio Code integration. For this service, users pay for the Azure compute resources used. 

#### Python Integration

You can leverage Azure SDK to interact with the Azure App App Services using Python. 

Microsoft Azure Web Apps Management Client Library **‘azure-mgmt-web’**

Authentication is needed and from the package, import WebSiteManagementClient. You can list and manage the resources, and deploy and manage the applications. 

### *Azure Functions*

#### About the Service

The cloud service can be used to build web APIs, respond to database changes, process IoT streams, and more so the user can focus on the code without worrying about deploying and maintaining servers. There are many features and integrations that allow the user to maintain less infrastructure without writing additional code. 

#### Python Integration

**Visual Studio Code** or another code editor and **Azure Functions Core Tools** are needed. The **Azure Functions extension** allows users to create a new Python Azure Functions project where they can write Python functions in separate files. This will define serverless functions. Azure Functions Core Tools can deploy Python Azure Functions to Azure and depending on the functions configuration, HTTP requests can be used to trigger Azure Functions for interaction after being deployed. 

# Databases

### *Azure SQL*

#### About the Service

This is a fully managed platform as a service (PaaS) database engine that allows users to focus on optimization activities, and domain-specific database administration by handling various database management functions, such as monitoring and backups. Users can process both relational data and non-relational structures within the SQL database while creating a high-performance data storage layer. 

#### Python Integration

Python SQL Driver **‘pyodbc’** has to be installed to connect to the Azure SQL Database using Python. This package serves as a data provider for database connection, command execution, and more. After connection configuration, SQL Queries can be executed using ‘cursor’, ‘execute’ for SQL commands, ect. 

### *Azure Confidential Ledger*

#### About the Service

This is a relatively recent and very secure service for users to manage sensitive data records as it runs on hardware-backed secure enclaves to guard against potential threats. The confidential ledger runs on a minimalist Trusted Computing Base (TCB) and provides data integrity features, such as tamper-proofing, and append-only operations which is suitable for storing business transaction records, operational IT and security events, ect. 

#### Python Integration

Azure Confidential Ledger client library **‘azure-confidentialledger’** and DefualtAzureCredential needs to be imported from ‘azure-identity’. Import control plane SDK and data plane SDK. Clients and ledgers can be created. Clients can be authenticated and DefaultAzureCredential will automatically handle many of the Azure SDK client scenarios. 
