# Practical 3: Word Count / Frequency Program using MapReduce in Hadoop

## Challenges Faced

1. Writing Mapper and Reducer scripts correctly to parse tokens and handle standard input/output streams.
2. Managing input and output directories in HDFS and ensuring the output directory does not already exist before running the Hadoop Streaming job.
3. Configuring and executing the Hadoop Streaming jar with proper mapper and reducer parameters.
4. Analyzing execution time differences across small, medium, and large datasets due to Hadoop startup and task initialization overhead.

## Solutions

1. Implemented `mapper.py` to tokenize words and emit `(word, 1)` pairs, and `reducer.py` to aggregate frequencies using standard Python `sys.stdin`.
2. Verified HDFS paths using `hdfs dfs -ls` and cleaned up existing output directories before execution using `hdfs dfs -rm -r`.
3. Used the Hadoop Streaming jar (`hadoop-streaming-*.jar`) with explicit `-file`, `-mapper`, and `-reducer` flags to ensure distributed execution across nodes.
4. Compared execution times across datasets, noting that fixed JVM startup and job scheduling overhead causes small differences on smaller datasets, while MapReduce scaling benefits become apparent on larger datasets.

---
