# Legacy-Retaill-ETL-Modernization

LEGACY RETAIL ETL MODERNIZATION
                 
END-TO-END DATA ENGINEERING FLOW

_________________________________________________________________
                  DATA SOURCES                         
_________________________________________________________________

   POS System        CRM Data        ERP/Inventory
 (SQL Server)       (MySQL)            (SAP)

        E-commerce API          Vendor Files
          (JSON/API)             (CSV/Excel)

                        |
                        |
_________________________________________________________________                         
                   DATA INGESTION LAYER                  
_________________________________________________________________

        Azure Data Factory (ADF)
        SSIS Migration / API Pipelines

 Tasks:
 ✔ Extract data from multiple sources
 ✔ Schedule daily/hourly pipelines
 ✔ Move raw data to cloud storage
                          
                         |
                         |
_________________________________________________________________
                     RAW DATA STORAGE                     
_________________________________________________________________
              Azure Data Lake Storage (ADLS)

              Raw Zone / Bronze Layer

                         |
                         |
_________________________________________________________________                 
                DATA TRANSFORMATION LAYER                │
_________________________________________________________________

                 Databricks + PySpark + SQL

 Tasks:
 ✔ Data cleansing
 ✔ Remove duplicates
 ✔ Null handling
 ✔ Join multiple datasets
 ✔ Standardize formats
 ✔ Business transformations

                         │
                         |
 _________________________________________________________________
                  CURATED DATA STORAGE                    
__________________________________________________________________
          Azure Synapse / Snowflake / SQL DW

                 Gold Layer / Data Warehouse

 Tables:
 ✔ Sales Fact Table
 ✔ Customer Dimension
 ✔ Product Dimension
 ✔ Inventory Summary

                          |
                          |
 _________________________________________________________________
                   REPORTING & ANALYTICS                  
 _________________________________________________________________

                      Power BI Dashboard

 Reports:
 ✔ Sales Performance
 ✔ Top Selling Products
 ✔ Inventory Status
 ✔ Customer Insights
 ✔ Regional Revenue Trends

                         |
                         |
 __________________________________________________________________
                     BUSINESS USERS                       
 __________________________________________________________________

      Management | Sales Team | Operations Team
