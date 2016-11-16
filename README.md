pyproc
===============

Process a data file and write metadata information to a data summary file.

    PyProc param.json

where the file param.json contains:

    {‘infile’:’C:/data/data.csv’,
    ‘metafile’:’C:/data/metadata.json’,
    ‘format’:’tabular’,
    ‘hasheader’:0,
    ‘separator’:’,’ }
    
This would make the program run and open the file data.csv and write the meta data it calculates to metadata.json. Included sample params files CSVcarsparams.json and JSONcarsparams.json. 

Example output:

    {
    "format": "tabular", 
    "fields": [
        {
            "Type": "string", 
            "Name": "Manufacturer", 
            "uniquevals": 3
        }, 
        {
            "Type": "string", 
            "Name": "Colour", 
            "uniquevals": 5
        }, 
        {
            "Type": "string", 
            "Name": "Size", 
            "uniquevals": 10
        }, 
        {
            "max": 95872.0, 
            "min": 26275.0, 
            "Type": "numeric", 
            "Name": "Milage", 
            "mean": 51752.0
        }, 
        {
            "max": 2907.0, 
            "min": 665.0, 
            "Type": "numeric", 
            "Name": "Price", 
            "mean": 1842.9239130434783
        }
    ], 
    "numrows": 100, 
    "header": 1, 
    "separator": ",", 
    "numfields": 5, 
    "infile": "carsdata.csv"
    }

Author: Emmanuel Osimosu
