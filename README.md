# pavan_cs-Data_Engineering-Assessment
PEI Group

## Prerequisite:
### Databricks
* Databricks Free Edition

### Install Required Python Package:
1. The openpyxl package is required to read Excel files into a PySpark DataFrame.
2. Run the following command in the first notebook cell:

    %pip install openpyxl==3.1.5

## Project Flow

1. **Import Required Packages**
   - Import Python and PySpark libraries.

2. **Read Order Data (JSON)**
   - Format price and numeric values.
   - Perform data type casting and schema validation.

3. **Read Customer Data (XLSX)**
   - Read Excel data using '**openpyxl**'.
   - Perform data type casting and schema validation.

4. **Read Product Data (CSV)**
   - Perform data type casting and schema validation.

5. **Create Bronze Delta Tables**
   - Save Orders, Customers, and Products DataFrames as Delta tables.
   - Execute unit tests to validate the Bronze tables.

6. **Perform Data Quality Checks**
   - Identify duplicate and null identifiers.
   - Validate phone numbers and postal codes.
   - Identify unmatched customer and product references.
   - Display data quality findings without modifying source records.

7. **Create Enriched Silver Tables**
   - Create the enriched Customer and Product table.
   - Create the enriched Order table with customer and product details.
   - Calculate Profit rounded to two decimal places.
   - Execute unit tests to validate the enriched tables.

8. **Create Profit Aggregation**
   - Aggregate profit by Year, Product Category, Product Subcategory, and Customer.
   - Save the results as a Delta table.

9. **Execute Spark SQL Queries**
   - Profit by Year.
   - Profit by Year and Product Category.
   - Profit by Customer.
   - Profit by Customer and Year.

## Overview on the workflow:
