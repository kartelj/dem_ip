# General information

This repository is related to paper Integer programing model for distance-edge-monitoring problem by Kratica, Filipovi\'c and Kartelj submitted to Yugoslav Journal of Operations Research. 
It contains three things:

1. test instances;
2. CPLEX binaries;
3. test results in .txt file.

# How to run binaries and reproduce results

You must have 64-bit version of Windows (tested on Windows 10). 

1. Download repository and unpack it. 
2. Position inside test directory. 
3. Run run_cplex.cmd. 

The results are appended to a file named out_cplex.txt. 

As can be seen from the content of run_cplex.cmd, the dem_cplex.exe requires four parameters:

```
dem_cplex.exe ../instances/random/NEW-V1000-P0.025-G0.txt 0 3600 0
```

These are:

1. the test instance absolute or relative path (with extension);
2. information on vertex and edge counting (0 means counting starts with zero, 1 means it starts with one);
3. the time limit in seconds;
4. the number of threads (0 sets automatically thread count to number of logical cores, while value >0 sets a specific thread count). 


