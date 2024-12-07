# PySpark Data Analysis Notebook

## Overview

This notebook demonstrates how to use PySpark for data analysis on a dataset containing employee information. It covers the entire process from setting up the Spark environment to performing various data transformations and analyses.

## Table of Contents

1. [Setup](#setup)
2. [Data Loading](#data-loading)
3. [Data Pre-Processing](#data-pre-processing)
4. [Data Analysis](#data-analysis)
5. [Conclusion](#conclusion)

## Setup

The notebook begins by installing the necessary PySpark library and setting up the environment variables required for Spark to run. It initializes a Spark session to enable data processing.

## Data Loading

The notebook checks for a local CSV file (`train.csv`). If it exists, it loads the data into a PySpark DataFrame. If not, it downloads the dataset from a specified URL and then loads it into the DataFrame.

## Data Pre-Processing

Data pre-processing steps include:
- Removing unnecessary characters from the 'Salary' column and converting it to an integer type.
- Lowercasing column names and replacing spaces with underscores.
- Converting the 'date_of_join' column from string format to date format.

## Data Analysis

The notebook performs several analyses on the employee data:

- How many people are in each job?

- How is the Gender Breakdown of the staff?

- What is the Age Spread?

- Which Job pays more?

- What does the staff headcount over time looks like?

- How is the Leave Balance Analysis conducted?

## Conclusion

The notebook concludes by stopping the Spark session, ensuring that resources are released. This analysis provides insights into employee demographics, salary distributions, and leave balances, which can be useful for HR and management decisions.

## Requirements

- Python 3.9 and above
- JDK - [link](https://www.oracle.com/in/java/technologies/downloads/)
- PySpark
- Jupyter Notebook

## Usage

To run this notebook, ensure you have the JDK and required libraries installed and execute the cells in order. Modify the dataset URL or local file path as needed for your environment.