# Benchmark on statistical tools for extreme value analysis.

## Exercise 1 : Cross-validation of open-source package for univariate extreme value analysis.

The purpose of this exercise is first to compare and cross validate open-source package implementing, basic, textbook, extreme value analysis (univariate, stationary). In a second-step, results obtain with in-house tools, and customized approach can be added. Two datasets representing quantities of interest in the maritime industry will be used. 

 - Time series of slamming loads on a ferry vessel.

 - Time series of significant wave height. 

 ### Quantities to calculate
 
For each of the dataset analysed, extremes on a given range of return periods are to be calculated, together with confidence intervals.

|                      | Slamming  | Wave height |
|--------------------- |---------- |-------------|
| Return period range  |  1e3 to 1e6s  | 1 to 100 years     |
| CI                   |  95%          |   95%       |

The results shall be provided with a CSV format, first columns being the return period, the second-one the return level estimate, the third one the lower bound of the CI interval, and the last the upper bound of the confidence interval. One results file per case / package / method should be provided, with the following convention: "packagename_casename_methodname.csv". 


 ### Part A prescribed settings for software cross validation.

To cross-validate the different packages, the settings are prescribed (threshold for POT, or block-size for block maxima approach). 

|                      | Slamming  | Wave height |
|--------------------- |---------- |-------------|
| Threshold (POT)      |   1200 kN     |   12.5m       |
| de-clustering windows  | 100s        |   2 days    |
| Block size (BM)      |  3500s        |   1 year    |


The scripts used to generate the results should be provided. An example is provided in the "Exercise_1" folder.

### Part B

In this second part, the objective is to discussed a wider range of approaches, ad'hoc method, as well as in-house code can be used. Quanties to calculate and format are the same as in part-A. Moreover, a description of the approach is requested. 
