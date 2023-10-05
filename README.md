# Car Crash Case Study #

This repository contains a set of Python scripts for the analysis of vehicle accidents happened across USA for a brief period of time. These scripts are designed to work together to load, analyze, and process data from different sources.

To get started with these scripts, follow the instructions below:

# Prerequisites
- Python 3.x
- PySpark
- Other dependencies as required in scripts

# Scripts

# 1. Table_Loading.py

This script contains two functions and a class for loading data into a PySpark DataFrame. This script includes two functions to load the schema definition from csv/json files and one class to create DataFrames with the specified schema.

### 2. Analysis.py

This script contains functions to perform various pre-defined analyses as per the requirement. Each function performs a specific analysis task, such as counting records, filtering data, or aggregating results.

# 3. Main.py

This script is the main entry point for running data analysis tasks. It readsthe configuration settings from a YAML file, loads data using the Table_Loading.py functions, and performs various analyses using the Analysis functions. The results of the analyses are written to an output file.

# Usage

1. Clone the repository to your local machine.
2. Install the required dependencies mentioned above in the Prerequisites section.
3. Edit the config_properties.yml file available in the config directory to specify your data sources, schema definitions, and output file configuration.

4. Run the Main.py script to execute the data loading and analysis tasks.

# Bash(spark-submit command)

spark-submit --name 'main_script' --master local[*] ./src/Main.py 2>&1 | tee ./data/logs/pyspark_logs.txt

# Result

Result of all the analysis will be written to the output file avaialble in output directory.
