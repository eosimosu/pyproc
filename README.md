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

Author: Emmanuel Osimosu
