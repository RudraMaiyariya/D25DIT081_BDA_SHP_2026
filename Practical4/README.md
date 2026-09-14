# Practical 4: Finding Maximum Temperature Recorded for Each Year using MapReduce

## Challenges Faced

1. Parsing unstructured or varying NCDC weather dataset records correctly to extract the exact year and temperature fields.
2. Handling missing, corrupted, or invalid temperature values present in large-scale raw climate datasets.
3. Managing data distribution, processing time, and resource consumption when running jobs over huge volumes of weather data.
4. Ensuring fault tolerance and verifying key-value pair emissions across Mapper and Reducer stages.

## Solutions

1. Developed a Mapper program to parse each line, extract the year as the key and temperature as the value, and output intermediate key-value pairs (`<Year, Temperature>`).
2. Filtered out corrupted/invalid temperature records during the Mapper phase before passing key-value pairs to the Reducer.
3. Uploaded the NCDC dataset into HDFS and utilized Hadoop's distributed storage and parallel MapReduce framework to speed up processing.
4. Implemented a Reducer to aggregate all temperature values per year, compare them, and output the maximum recorded temperature for each year to HDFS.

---
