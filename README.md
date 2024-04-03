
# sales_project_adf

Sample project to use ADF, ADLS Gen2 and 

To read three input files (Sales, Product, customer) and ingest, transform and Load by following medallion Architecture   (Bronze, Silver & Gold layers)

Data flow
----------
**Step 1** : Copy the data from external landing container (data-ext-landing) to raw container (data-raw-bronze) - Used Copy data, delete activities


Inputs
------
Sales - Sales information of each order
Product - Product specific data (Product ID, name, family )
Customer - Customer data (Customer ID, name etc)

Outputs
-------
Fast Moving product
Total Sales per day


Dataset formats
---------------
1. Delimited (csv)
2. parquet

Linked Services
---------------
1. Azure Data Lake Storage Gen 2

Trigger types
---------------
1. Scheduled 
2. Storage event


Activities used
---------------
1. Copy Data
2. Dataflow
3. Execute Dataflow
4. Delete Activity
5. Pipeline
6. Execute Pipeline

Dataflow Transformations
------------------------
1. Aggregate Transformation
2. Derived column Transformation
3. Conditional Split Transformation
4. Join Transformation
5. Select Transformation
6. Sort Transformation
7. Source Transformation
8. Sink Transformation

