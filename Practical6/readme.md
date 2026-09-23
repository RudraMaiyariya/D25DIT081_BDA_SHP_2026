# Practical 6: E-Commerce Sales Analysis using Spark DataFrames

## Challenges Faced

1. Loading the sales data into a Spark DataFrame and checking the dataset structure and schema.

2. Creating the Revenue column using Quantity_Sold and Unit_Price and performing different sales calculations.

3. Performing category-wise, product-wise, and region-wise analysis using Spark DataFrame operations.

## Solutions

1. Loaded the sales_data.csv file using Spark and validated the columns, data types, rows, and missing values.

2. Created the Revenue column and used groupBy(), sum(), avg(), and orderBy() for sales analysis.

3. Identified top-selling products, revenue-generating regions, and the highest-revenue category, which was Clothing.
