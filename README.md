# Home_Sales
Module 22 Challenge

![housing-market-home-sales-real-estate](https://github.com/user-attachments/assets/1c6b52ae-a7c7-45c8-ae75-6ff214ed932c)
*Image credit: [pymnts.com](https://www.pymnts.com/real-estate/2020/us-home-sales-hit-highest-january-peak-in-years/)*

# Overview
In this challenge, I have used my knowledge of SparkSQL to determine key metrics about home sales data. Then I used Spark to create temporary views, partition the data, cache and uncache a temporary table, and verified that the table has been uncached.

# Instructions
- Rename the Home_Sales_starter_code.ipynb file as Home_Sales.ipynb.
- Import the necessary PySpark SQL functions for this assignment.
- Read the home_sales_revised.csv data in the starter code into a Spark DataFrame.
- Create a temporary table called home_sales.
- Cache your temporary table home_sales.
- Check if your temporary table is cached.
- Using the cached data, run the last query that calculates the average price of a home per "view" rating having an average home price greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.
- Partition by the "date_built" field on the formatted parquet home sales data.
- Create a temporary table for the parquet data.
- Run the last query that calculates the average price of a home per "view" rating having an average home price greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.
- Uncache the home_sales temporary table.
- Verify that the home_sales temporary table is uncached using PySpark.
- Download your Home_Sales.ipynb file and upload it into your "Home_Sales" GitHub repository.

# Answer the following questions using SparkSQL:

*?* -  What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.

*A*- <img src="https://github.com/user-attachments/assets/99833278-391b-492c-9567-d7292ee611b6" alt="Screenshot 2024-08-16 151625" width="300"/>

*?* - What is the average price of a home for each year the home was built, that has three bedrooms and three bathrooms? Round off your answer to two decimal places.

*A*- <img src="https://github.com/user-attachments/assets/7020322d-8f6d-4514-ba7f-e040d6f111db" alt="Screenshot 2024-08-16 151625" width="300"/>
  
*?* - What is the average price of a home for each year the home was built, that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.

*A*- <img src="https://github.com/user-attachments/assets/ac59c816-497c-4497-a2e2-5bc4d3fc24f5" alt="Screenshot 2024-08-16 151625" width="300"/>

*?* - What is the average price of a home per "view" rating having an average home price greater than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.

*A*- <img src="https://github.com/user-attachments/assets/0e25b04e-c6c9-41cd-9227-f11fb942d090" alt="Screenshot 2024-08-16 151625" width="200"/>

# Support and Resources


# Requirements
- A Spark DataFrame is created from the dataset. (5 points)
- A temporary table of the original DataFrame is created. (10 points)
- A query is written that returns the average price, rounded to two decimal places, for a four-bedroom house that was sold in each year. (5 points)
- A query is written that returns the average price, rounded to two decimal places, of a home that has three bedrooms and three bathrooms for each year the home was built. (5 points)
- A query is written that returns the average price of a home with three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet for each year the home was built rounded to two decimal places. (5 points)
- A query is written that returns the average price of a home per "view" rating having an average home price greater than or equal to $350,000, rounded to two decimal places. (The output shows the run time for this query.) (10 points)
- A cache of the temporary "home_sales" table is created and validated. (10 points)
- The query from step 6 is run on the cached temporary table, and the run time is computed. (10 points)
- A partition of the home sales dataset by the "date_built" field is created, and the formatted parquet data is read. (10 points)
- A temporary table of the parquet data is created. (10 points)
- The query from step 6 is run on the parquet temporary table, and the run time is computed. (10 points)
- The "home_sales" temporary table is uncached and verified. (10 points)
