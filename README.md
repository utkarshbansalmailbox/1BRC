# Data Processing with Dask

## Overview
This repository contains scripts for generating and processing large datasets using Dask, which leverages Pandas for parallel computing. The primary objective is to demonstrate the efficiency and capability of Dask in handling and analyzing large-scale data.

## Project Task
The main task of this project is to compute the minimum, maximum, and mean of 1 billion rows. Dask is used instead of Polars to generate the dataframe and perform the computations.

## Data Folder Contents
The `data` folder contains the following files:
1. **createMeasurements.py**: The original script for generating data.
2. **createMeasurements2.py**: Modified version of the script to produce a CSV file instead of a semi-colon separated text file.

## File Configuration
Data is generated using `createMeasurements2.py`, resulting in the following file **measurements.csv** with a -**file size of 13.8 GB**:

## Performance Metrics
### Time to Produce File
- **CPU Times**:
  - User: 2.42 s
  - System: 839 ms
  - Total: 3.26 s
- **Wall Time**: 3min 14s

### Time to Parse Data in File
- **CPU Times**:
  - User: 9.24 ms
  - System: 3.43 ms
  - Total: 12.7 ms
- **Wall Time**: 56.1 ms

### Time to Calculate Min, Max, Mean
- **CPU Times**:
  - User: 2min 56s
  - System: 16.3 s
  - Total: 3min 12s
- **Wall Time**: 1min 22s

## Working
This project leverages the power of Dask dataframes to handle large datasets efficiently. The scripts demonstrate the process of generating, storing, and analyzing data, highlighting the performance benefits of parallel computing.

### Result
### Steps to Run
1. **Generate Data**:
   ```sh
   python createMeasurements2.py
   ```
2. **Process Data**:
  Used Dask functions to load and calculate min, max & mean of the data as per your requirements.

  **info:**
  Initial number of rows: 1000000000
  Number of rows after groupby and aggregate: 413

## Dependencies

1.  Dask
2.  Pandas

**Install the dependencies using**:
  ```sh
  Copy code
  pip install dask pandas
```

## Conclusion

  This repository showcases the capabilities of Dask in managing large datasets with ease. The provided scripts and performance metrics serve as a reference for utilizing parallel computing in data analysis tasks.
