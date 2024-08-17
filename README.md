# Hadoop MapReduce Word Count Project

This repository contains files for a Hadoop MapReduce word count project, implemented as part of a homework assignment.

## Files in this Repository

1. `MapReduce_Hadoop_Homework.ipynb`: Jupyter notebook containing the main project code and documentation.

2. `hdfs-wordcount.txt`: Output file containing word count results from HDFS.

3. `mapper.py`: Python script for the mapper function of the MapReduce job.

4. `pembukaan_uud1945.txt`: Input text file, the preamble of the 1945 Indonesian Constitution.

5. `reducer.py`: Python script for the reducer function of the MapReduce job.

## Project Overview

This project implements a word count application using Hadoop MapReduce. It processes the text from `pembukaan_uud1945.txt`, counts the occurrences of each word, and outputs the results.

### How it Works

1. The mapper (`mapper.py`) reads input text and emits key-value pairs of (word, 1).
2. The reducer (`reducer.py`) aggregates these counts for each unique word.
3. The final output is stored in `hdfs-wordcount.txt`.

## Usage

To run this MapReduce job:

1. Ensure Hadoop is properly set up and running.
2. Put the input file into HDFS.
3. Run the MapReduce job using the Hadoop Streaming API with `mapper.py` and `reducer.py`.
4. Check the output in `hdfs-wordcount.txt`.

Detailed instructions and code execution can be found in the `MapReduce_Hadoop_Homework.ipynb` notebook.

## Requirements

- Python
- Jupyter Notebook (for viewing and running the .ipynb file)
