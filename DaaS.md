### Data-as-a-Service

_Data as a service (DaaS) is a business model where data is made available on demand and regardless of the consumer’s location or infrastructure. To enable DaaS, organizations provide cloud-based software for analyzing and managing the accessed data._
Credit: [MongoDB](https://www.mongodb.com/initiatives/data-as-a-service#:~:text=Data%20as%20a%20service%20(DaaS)%20is%20a%20business%20model%20where,the%20consumer's%20location%20or%20infrastructure.)

## DaaS in Azure (Step 1: Data Ingestion, Processing & Transformation)

![image](https://github.com/roime81/roime81/assets/7858481/3d8c66db-9cea-465d-ab39-a3c7048d4678)

* To have DaaS in Azure, diagram above used to implement end-to-end data ingestion and processing. Assumed data are ingested from on-prem database server, Azure Data Factory used to establish ingestion pipelines.
* Data will transformed from from raw to curated / processed in Data Factory. Data then saved in SQL database.  
* Besides ADF, Databricks can be used to ingest data, using Python or R.
* Since there are more than 1 pipelines and severals curated data stored, Synapse is used to form a DWH, that aggregates, integrates multiple curated data sources.
* End users than connected to Synapse using data endpoint created.
* Besides SQL, data also can be stored in preferred storage e.g PostgreSQL, Blob, Data Lake.

## DaaS in Azure (Step 2: Data Integration, Scanning & Mapping)

![image](https://github.com/roime81/roime81/assets/7858481/b9c3b6dc-cdd8-40fc-8f68-e98a92904221)


### Further Reading

* [Data-as-a-Service (1)](https://builtin.com/big-data/data-as-a-service-daas)
* [Data-as-a-Service (2)](https://www.techtarget.com/searchdatamanagement/definition/data-as-a-service)
* [Data-as-a-Service (3)](https://www.teradata.com/insights/cloud-data-analytics/data-as-a-service)

### Some Reference Architecture

* [Azure](https://techcommunity.microsoft.com/t5/azure-architecture-blog/designing-and-implementing-modern-data-architecture-on-azure/ba-p/3440322)
* [AWS](https://aws.amazon.com/blogs/architecture/lets-architect-modern-data-architectures/)
* [GCP-Ritwick Dutta](https://www.linkedin.com/pulse/gcp-enterprise-data-solution-architecture-how-integrate-dutta/)
