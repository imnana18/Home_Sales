# Home Sales Analysis 🏠


## Overview

This project involved using `SparkSQL` to perform various operations on home sales data such as creating `temporary views`, `partitioning data`, `caching and uncaching` temporary tables, saving and viewing `parquet` files, and running queries to answer questions about the home sales DataFrame.


### Files

Downloaded project files from [Module 22 Challenge](https://static.bc-edx.com/data/dl-1-2/m22/lms/starter/Starter_Code.zip).


### Process

1. Renamed the `Home_Sales_starter_code.ipynb` file to `Home_Sales.ipynb`.
2. Imported necessary `PySpark SQL` functions for the assignment.
3. Read the `home_sales_revised.csv` data into a `Spark DataFrame`.
4. Created a `temporary table` named `home_sales`.
5. Answered the following questions using `SparkSQL` (please reference code for specific queries):
    - Determined the average price for a four-bedroom house sold for each year.
      
      ![Screenshot 2024-04-03 at 02 50 17](https://github.com/imnana18/Home_Sales/assets/147445115/e197a008-ac41-4bd1-be6c-86d499d16432)

    - Calculated the average price of a home for each year the home was built, considering three bedrooms and three bathrooms.

      ![Screenshot 2024-04-03 at 02 49 50](https://github.com/imnana18/Home_Sales/assets/147445115/fb74bb7a-fd67-4a20-abc8-0c1ee605a3ba)
      
    - Computed the average price of a home for each year the home was built, with specific criteria on bedrooms, bathrooms, floors, and square footage.
      
      ![Screenshot 2024-04-03 at 02 51 58](https://github.com/imnana18/Home_Sales/assets/147445115/ead35ed0-4da3-4d1a-8e40-19bc1ea0ec89)

    - Analyzed the average price of a home per "view" rating with an average home price greater than or equal to $350,000, including determining query runtime.

      ![Screenshot 2024-04-03 at 02 52 26](https://github.com/imnana18/Home_Sales/assets/147445115/d27da781-01e7-4d28-95e6-67acb1dff50d)

6. `Cached` the temporary table `home_sales`.
7. Checked if the temporary table is cached.
8. Ran the last query in step 5 using the cached data, determining `runtime` and comparing it to uncached runtime.
9. Partitioned the formatted `parquet` home sales data by the "date_built" field.
10. Created a temporary table for the parquet data.
11. Ran the last query in step 5 using the partitioned parquet data, determining runtime and comparing it to uncached runtime.
12. `Uncached` the home_sales temporary table.
13. Verified that the home_sales temporary table is uncached using `PySpark`.


### References

Data for this dataset was generated by edX Boot Camps LLC, and is intended for educational purposes only.
 
