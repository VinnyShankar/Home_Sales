# Home_Sales

## Credits
- Author: Vinny Shankar
- Acknowledgements:
    - Study Groups: worked together with several students to understand the assignment
    - Students: [Hany Dief](https://github.com/hanydief)
    - Program: University of California Berkeley Data Analytics Bootcamp
    - Starter Code: The Module Challenge provided starter code that guided the process
    - Tutor: [Bethany Lindberg](https://github.com/bethanylindberg)
    - Instructor: Ahmad Sweed

## Note about Google Colab

The notebook in this repository is meant to be run in Google Colab: https://colab.research.google.com/

## Overview

This project uses SparkSQL to determine key metrics about home sales data. Spark is used to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.

## Detailed Steps

A Spark DataFrame is created from the dataset.

A temporary table of the original DataFrame is created.

A query is written that returns the average price, rounded to two decimal places, for a four-bedroom house that was sold in each year.

A query is written that returns the average price, rounded to two decimal places, of a home that has three bedrooms and three bathrooms.

A query is written that returns the average price of a home with three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet for each year built rounded to two decimal places.

A query is written that returns the view rating for the average price for homes that are greater than or equal to $350,000, rounded to two decimal places. (The output shows the run time for this query.)

A cache of the temporary "home_sales" table is created and validated.

The query from step 6 is run on the cached temporary table, and the run time is computed.

A partition of the home sales dataset by the "date_built" field is created, and the formatted parquet data is read.

A temporary table of the parquet data is created.

The query from step 6 is run on the parquet temporary table, and the run time is computed.

The "home_sales" temporary table is uncached and verified.