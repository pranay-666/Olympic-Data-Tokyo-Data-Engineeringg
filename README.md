# Olympic-Data-Tokyo-Data-Engineering
## Introduction
This project implements a scalable data engineering pipeline for Olympic data using Microsoft Azure services. It covers the full data lifecycle from ingestion to analysis, focusing on the 2021 Tokyo Olympics dataset.
## Architecture Overview
The project uses the following Azure services:
![alt text](https://github.com/pranay-666/Olympic-Data-Tokyo-Data-Engineeringg/blob/main/images/Design.png?raw=true)

- Azure Data Factory: For data ingestion.
- Azure Data Lake Storage Gen2: To store raw and transformed data.
- Azure Databricks: For data transformation and cleaning.
- Azure Synapse Analytics: For data analysis and visualization.
## Data Flow
1.	**Data Source:** 2021 Tokyo Olympics dataset (Kaggle).
2.	**Data Ingestion:** Azure Data Factory ingests the raw CSV files from Kaggle.
3.	**Raw Data Storage:** Stored in Azure Data Lake Gen2.
![alt text](https://github.com/pranay-666/Olympic-Data-Tokyo-Data-Engineeringg/blob/main/images/RawData.png?raw=true)
4.	**Data Transformation:** Azure Databricks processes and cleans the data.
6.	**Transformed Data Storage:** Cleaned data is stored in Azure Data Lake Gen2.
![alt text](https://github.com/pranay-666/Olympic-Data-Tokyo-Data-Engineeringg/blob/main/images/TransformedData.png?raw=true)
7.	**Analytics:** Insights are generated using Azure Synapse Analytics.
### Dataset
The project uses a Kaggle dataset with information about:

* Athletes
* Coaches
* Gender-wise participation
* Medal statistics
* Team composition
## Key Steps
1. **Resource Group Setup:** Resource groups are configured in Azure to manage the connections between different services used in the project
![alt text](https://github.com/pranay-666/Olympic-Data-Tokyo-Data-Engineeringg/blob/main/images/ResourceGroups.png?raw=true)
2.	**Storage Setup:** Create Azure Storage Accounts to securely store large data volumes.
![alt text](https://github.com/pranay-666/Olympic-Data-Tokyo-Data-Engineeringg/blob/main/images/StorageAccounts.png?raw=true)
3. ****Container Setup:**  Storage containers are utilized to separate the different datasets related to the 2021 Tokyo Olympics, ensuring that the data remains organized and easily accessible.
![alt text](https://github.com/pranay-666/Olympic-Data-Tokyo-Data-Engineeringg/blob/main/images/Container.png?raw=true)
5.	**Data Ingestion:** Use Azure Data Factory to automate CSV file ingestion.
![alt text](https://github.com/pranay-666/Olympic-Data-Tokyo-Data-Engineeringg/blob/main/images/AzureDataFactory.png?raw=true)
6.	**Data Transformation:** Clean and normalize data in Azure Databricks.
![alt text](https://github.com/pranay-666/Olympic-Data-Tokyo-Data-Engineeringg/blob/main/images/AzureDatabricks.png?raw=true)
8.	**Data Analysis:** Generate insights with Azure Synapse Analytics.
![alt text](https://github.com/pranay-666/Olympic-Data-Tokyo-Data-Engineeringg/blob/main/images/SynapseAnalytics.png?raw=true)
## Insights
*	Athlete Participation: Analyze athlete counts by country to assess sports investment.
  * Line Graph:
 	![alt text](https://github.com/pranay-666/Olympic-Data-Tokyo-Data-Engineeringg/blob/main/images/Query1.jpeg?raw=true)
*	Medal Tally: Evaluate each country’s performance by total medals won.
  * Bar Graph:
 	![alt text](https://github.com/pranay-666/Olympic-Data-Tokyo-Data-Engineeringg/blob/main/images/Query2-1.jpeg?raw=true)
  * Area Graph:
  ![alt text](https://github.com/pranay-666/Olympic-Data-Tokyo-Data-Engineeringg/blob/main/images/Query2-2.jpeg?raw=true)
*	Gender Participation: Explore gender representation across Olympic disciplines.
  * Line Graph:
 	![alt text](https://github.com/pranay-666/Olympic-Data-Tokyo-Data-Engineeringg/blob/main/images/Query3-1.jpeg?raw=true)
  * Bar Graph:
  ![alt text](https://github.com/pranay-666/Olympic-Data-Tokyo-Data-Engineeringg/blob/main/images/Query3-2.jpeg?raw=true)
  * Area Graph:
  ![alt text](https://github.com/pranay-666/Olympic-Data-Tokyo-Data-Engineeringg/blob/main/images/Query3-3.jpeg?raw=true)
## Technologies Used
*	Azure Services: Data Factory, Data Lake Gen2, Azure Databricks, Synapse Analytics
*	Programming: Python, SQL, Pyspark
## Future Work
* Investigate the correlation between athlete participation and medal success.
## How to Execute
*	Clone the repository.
*	Set up the Azure environment (Storage Accounts, Linked Services, Resource Groups).
*	Run the pipeline to ingest, transform, and analyze the data.
## Contributors
**Pranay Reddy Kodumuru**
## Credits
Darshil Parmar and Rohit Annasaheb Ragde
## References
https://www.youtube.com/watch?v=IaA9YNlg5hM&t=41s
