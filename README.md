Data folder  containts 2 files:
    1. createMeasurements.py  – original file
    2. createMeasurements2.py – changed code to produce .csv instead of semi-colon seperated txt file.

Used dask dataframe whih uses pandas in backend with parallel computing capabilities.
File configs (data generated from createMeasurements2.py):
1. file size: 13.8 GB
2. time to produce file:
    > CPU times: user 2.42 s, sys: 839 ms, total: 3.26 s
    > Wall time: 3min 14s
3. time to parse data in file:
    > CPU times: user 9.24 ms, sys: 3.43 ms, total: 12.7 ms
    > Wall time: 56.1 ms
4. time to calulate min, max, mean:
    > CPU times: user 2min 56s, sys: 16.3 s, total: 3min 12s
    > Wall time: 1min 22s


Working: 


