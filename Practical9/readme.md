# Practical 9: Social Media Trend Detection Using PySpark

## Challenges Faced

1. Loading and validating the social media hashtag dataset using PySpark DataFrames.
2. Grouping hashtags and calculating their frequency to identify popular and trending topics.
3. Performing daily, regional, and category-wise trend analysis using Spark transformations and aggregations.
4. Generating a visualization of the most frequently used hashtags using Matplotlib.

## Solutions

1. Loaded the social media hashtag dataset into a Spark DataFrame and displayed its schema and sample records.
2. Used `groupBy()`, `count()`, and `orderBy()` to calculate hashtag frequency and rank popular hashtags.
3. Used Window functions to identify daily and regional trending hashtags and categorized hashtags into Technology, Sports, and Entertainment.
4. Generated a bar chart of the top trending hashtags and completed the final social media trend analysis report.
