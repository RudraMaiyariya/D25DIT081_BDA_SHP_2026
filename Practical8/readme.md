# Practical 8: Stock Market Analytics Using Window-Based Analysis

## Challenges Faced

1. Loading the stock market dataset into a Spark DataFrame and checking the schema, records, and data types.
2. Grouping stock records using the `Symbol` column and calculating average, maximum, and minimum closing prices.
3. Sorting the stock summary to identify stocks with the highest average and maximum closing prices.
4. Generating an overall stock price summary and interpreting the calculated market data.

## Solutions

1. Loaded the stock market CSV file into a Spark DataFrame and displayed the dataset structure and sample records.
2. Used `groupBy()` with `avg()`, `max()`, and `min()` to generate a summary for each stock symbol.
3. Used `orderBy()` to sort stocks according to average and maximum closing prices and displayed the required results.
4. Calculated the overall average, maximum, and minimum closing prices to generate a simple stock market summary report.
5. Displayed the stocks with the highest average closing prices as part of the stock performance analysis.
