Getting and Cleaning Data - Coursera Project

This is the course project for Getting and Cleaning Data course on Coursera. Code is written in R in file. Source file is run_analysis.R. This R script does the following things:

Download the dataset if it does not already exist in the working directory.

Checks if zip has already been downloaded in ./UCI HAR Dataset directory?
Checks if zip has already been unzipped?
List all the files of UCI HAR Dataset folder The files that will be used to load data are listed as follows: test/subject_test.txt test/X_test.txt test/y_test.txt train/subject_train.txt train/X_train.txt train/y_train.txt

Loads activity, subject and feature info. Reads data from the files into the variables.

Reads the Activity files.
Reads the Subject files.
Reads Features files.
Merges the training and the test sets to create one data set.

Concatenates the data tables by rows.
set names to variables.
Merges columns to get the data frame Data for all data.
Extracts only the measurements on the mean and standard deviation for each measurement.

Subsets Name of Features by measurements on the mean and standard deviation.
Subsets the data frame Data by selected names of Features.
Uses descriptive activity names to name the activities in the data set.

Reads descriptive activity names from activity_labels.txt
Factorizes variable activity in the data frame Data using descriptive activity names.
Appropriately labels the data set with descriptive variable names.

Creates an independent tidy dataset that consists of the average (mean) value of each variable for each subject and activity pair.

Final output file is tidydata.txt