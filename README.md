#Welcome to the UCI Smartphone Data: Tidying Scipt

## AIM: What does the script do?
[run_analysis.R](run_analysis.R) tidies the human activity data '[UCI Human Activity Recognition by Smartphone] 
(http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones)'

## INSTRUCTIONS: How do I use it?
1. Download the data files from the [UCI lab server] or [Coursera Get-and-Clean Data] 
2. Unzip the files in your working directory. A typically unzips to a folder *UCI HAR Dataset*
3. Download [run_analysis.R](run_analysis.R) to the working directory.
4. Ensure both [run_analysis.R](run_analysis.R) and the source data folder *UCI HAR Dataset* are at the same level.
5. Source the R script in R or RStudio to autorun and tidy the data set.  

## METHOD: How does it tidy the data?
- PRE-FLIGHT CHECKS: Ensure the UCI data is unzipped in the working directory, loads required libraries
- STEP 1: **Merge test and trials data** folders into a single data frame, use **descriptive activity names**, **one variable per column**, and **one observation per row**
- STEP 2: Subset the merged data to keep only the **means and standard deviation** variables
- STEP 3: Replace variable (column) names with **human readable variable names**
- FINISH-UP: **Generate tidy data text file** with data/time in the filename.  


## Requirements
The script has been tested in RStudio with *R version 3.2.0 'Full of Ingredients'*
Packages: *plyr, dplyr, reshape2* must be installed

## Output
The tidy data set looks like this: [UCI_Smartphone_data_tidy.txt](UCI_Smartphone_data_tidy.txt) (~11Mb)
Thanks!
@vic_divecha
