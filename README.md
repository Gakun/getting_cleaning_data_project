# Getting and cleaning the UCI HAR Dataset
This Repo provides a method to cleaning and summarizing the UCI HAR Dataset

## Brief of cleaning method
1. Read the test dataset and training datasets. Extract only the measurements on the mean and standard deviation for each measurement of two datasets.
2. Add the subject id, activities id and set labels (test or train) to the two dataset
3. Combine the test and training datasets
4. Labels the data set with descriptive variable names using provided activity labels
5. Calculate the average of each variable for each activity and each suject, save the result as a txt file.

## Files contained in the repo
1. README.md
2. CodeBook.md: Describes the variables and the steps to clean up the data
3. run_analysis.R: R script to run the cleaning process
4. data_sum.txt: The final output data of the average of each variable for each activity and each subject
