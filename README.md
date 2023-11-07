# capstone Project
A data Engineer project involves Azure Data Factory, Azure synapse analytics,Azure Data Lake, Azure Data Bricks, Azure active directory, Azure key vault and power BI
# achitecture
<img width="1474" alt="截屏2023-10-29 22 17 10" src="https://github.com/Felicia1993/milestoneProject/assets/22839284/7fa885aa-b46a-400a-9a7d-44d07e7e89bd">

## Environment setup
The first step is to create a storage account, in order to use Data Lake Gen2 as the storage, when creating the storage account, the performance should select Premium and Premium account type choose as Block Blobs. Otherwise, An error would happend during data ingestion. 
## Data ingestion
The dataset is from Kaggle 2021 Olympic in Tokyo https://www.kaggle.com/datasets/arjunprasadsarkhel/2021-olympics-in-tokyo/data. Import the excel data into mysql.   
### Method 1
Firstly, download dataset from Kaggle and import them into MySQL. Then, create integration runtime by newing self-hosted on Azure and register the runtime ingestion to your on-premises server, in order to load data from on-premises MySQL to Data Lake Gen2. 
### Method 2
Copy data from HTTP source by creating copy-data pipeline and define the source and destination of your data. Source is from HTTP dataset and load data to Data Lake Gen2.

## Data storage
The data is stored in Azure Data lake Gen2.         
### Different layers of Azure data lake      
Bronze layer: it has an exact copy of what the data looks like in this data source. If something goes wrong, you can come back to the broze layer and get all the data to try out which is goint to be the same as the data source.     
silver layer: When data loads into bronze layer, use databricks to do some transformation, and load the transformation data into silver layer. 
gold layer: Different level of transformation, stores final cleanest forms for data  
## Data transformation
Once the data added into Data Lake, Databricks is used to transformation the row data into the most  
## Data Loading     
## Data reporting
## End to End pipeline testing




