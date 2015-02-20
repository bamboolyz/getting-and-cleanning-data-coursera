Getting and Cleaning Data 
==========================
This file describes how run_analysis.R script works.
* Unzip the data from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip and rename the folder as "uciData".
* Set the folder "uciData" as the working directory and save the "run_analysis.R" script within "uciData".
* Call source("run_analysis.R") in RStudio. 
* Two output files will be generated in the current working directory:
  - merged_clean_data.txt (8.2 Mb) & data_set_with_the_averages.txt (220 Kb)
* Use data <- read.table("data_set_with_the_averages.txt") to read the data. It is 180x68 because there are 30 subjects and 6 activities, thus "for each activity and each subject" means 30 * 6 = 180 rows. Note that the provided R script has no assumptions on numbers of records, only on locations of files.