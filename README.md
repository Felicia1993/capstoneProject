# milestone Project
A data Engineer project involves Azure Data Factory, Azure synapse analytics,Azure Data Lake, Azure Data Bricks, Azure active directory, Azure key vault and power BI
# achitecture
<img width="1436" alt="截屏2023-10-29 22 12 16" src="https://github.com/Felicia1993/milestoneProject/assets/22839284/20d03340-16f0-4bc4-aaa7-0a8a16ff1304">    

## Data ingestion
Azure data factory used to connect with on-premises SQL server database to copy all the table from the database and move all the table to the cloud.     
## Data storage
The data is stored in Azure Data lake Gen2.         
### Different layers of Azure data lake      
Bronze layer: it has an exact copy of what the data looks like in this data source. If something goes wrong, you can come back to the broze layer and get all the data to try out which is goint to be the same as the data source.     
silver layer: When data loads into bronze layer, use databricks to do some transformation, and load the transformation data into silver layer. 
gold layer: Different level of transformation, stores final cleanest forms for data
## Data analytics    
## Data visualization     



## Data transformation
Once the data added into Data Lake, we use Databricks to transformation the row data into the most  
