# Practical 7: Performance Optimization Using Caching and Partitioning

## Challenges Faced

1. Loading the movie ratings dataset into a Spark DataFrame and checking its schema and number of partitions.
2. Measuring the execution time of an average rating calculation before applying optimization.
3. Applying `cache()` and using `count()` to load the dataset into memory before running the analysis again.
4. Repartitioning the dataset and comparing execution times before and after optimization.

## Solutions

1. Loaded the movie ratings CSV file into a Spark DataFrame and displayed the schema, records, and partition count.
2. Calculated the average movie rating and recorded the execution time before optimization.
3. Applied `cache()` to the DataFrame and triggered caching using `count()` before calculating the average rating again.
4. Repartitioned the dataset into 4 partitions and measured the execution time after repartitioning.
5. Generated a performance report comparing execution time before caching, after caching, and after repartitioning.
