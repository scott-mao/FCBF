Fast Correlation-Based Feature (FCBF) selection.
====

Paper: http://www.public.asu.edu/~huanliu/papers/icml03.pdf

Implementation of the FCBF algorithm. 

Usage: 

  In Python, call 
  
    fcbf_wrapper(inpath, thresh, delim=',', header=False, classAt=-1)
  
  OR
  
  From command line, 
  
    > python fcbf.py -h
    usage: fcbf.py [-h] [-inpath] [-thresh] [-delim] [-header] [-classAt]
    
    Fast Correlation-Based Feature Selection (FCBF)
    
    optional arguments:
      -h, --help  show this help message and exit
      -inpath     Path to input file
      -thresh     SU threshold
      -delim      File delimiter
      -header     Contains header?
      -classAt    Index of class column
    
    > python fcbf.py -inpath='../data/lungcancer.csv' -thresh=0.05
    Reading file. Please wait ...
    Success! Dimensions: 32 x 57
    Performing FCBF selection. Please wait ...
    Done!
    
    #Features selected: 6
    Selected feature indices:
    [[  0.32054501  39.        ]
     [  0.32017586  19.        ]
     [  0.19562365  55.        ]
     [  0.15251083   1.        ]
     [  0.12478091   9.        ]
     [  0.07640196   2.        ]]
    
    File saved successfully. Path: ../data/features_lungcancer.csv
    
