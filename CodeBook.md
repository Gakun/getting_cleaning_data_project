## Explaination of the Script
1. Read the features.txt file
2. Use regex to find the position of features contains mean() or std()
3. Read the X_test.txt file and assign to the testData.
4. Select the columns based on the feature position that found in step 2
5. Change the column name to the feature name
6. Read the subject_test.txt and y_test.txt to get the subject id and activity id of each data row
7. Bind the subject id column and activity id column to the testData.
8. Add the set column to testData, whose value is test for all rows
9. repeat step 3-8 on training dataset. In the step 8, the value of set column is train
Extract only the measurements on the mean and standard deviation for each measurement of two datasets.
10. Combine the testData and trainData and assign to data
11. Read the activity_labels.txt to get activity id and corresponding activity name and assign to labels
12. Merge the data with labels on the column activity, and remove the activity column from the result
13. Labels the data set with descriptive variable names using provided activity labels
14. Use the dplyr to group the data by activity_name and subject, summarise all columns using mean function
15. Save the result as data_sum.txt without row names

## Description of the output data variables
The output data contains 68 variables and 180 observations. Each observation refers to the mean of all measurements for each activity and subject combinations.

The list of all variables and descriptions as follows:
### Factors
1. activity_name: The labels of activity performed in the test

2. subject: The id of the subject
### Measurements
The measurements variables are selected from UCI HAR Dataset. Only the mean and standard deviation are selected. All the measurements are the mean value of the original data for each activity and subject combinations.
3. tBodyAcc-mean()-X 

4. tBodyAcc-mean()-Y 
5. tBodyAcc-mean()-Z
6. tBodyAcc-std()-X
7. tBodyAcc-std()-Y 
8. tBodyAcc-std()-Z 
9. tGravityAcc-mean()-X 
10. tGravityAcc-mean()-Y 
11. tGravityAcc-mean()-Z 
12. tGravityAcc-std()-X 
13. tGravityAcc-std()-Y 
14. tGravityAcc-std()-Z 
15. tBodyAccJerk-mean()-X 
16. tBodyAccJerk-mean()-Y 
17. tBodyAccJerk-mean()-Z 
18. tBodyAccJerk-std()-X 
19. tBodyAccJerk-std()-Y 
20. tBodyAccJerk-std()-Z 
21. tBodyGyro-mean()-X 
22. tBodyGyro-mean()-Y 
23. tBodyGyro-mean()-Z 
24. tBodyGyro-std()-X 
25. tBodyGyro-std()-Y 
26. tBodyGyro-std()-Z 
27. tBodyGyroJerk-mean()-X 
28. tBodyGyroJerk-mean()-Y 
29. tBodyGyroJerk-mean()-Z 
30. tBodyGyroJerk-std()-X 
31. tBodyGyroJerk-std()-Y 
32. tBodyGyroJerk-std()-Z 
33. tBodyAccMag-mean() 
34. tBodyAccMag-std() 
35. tGravityAccMag-mean() 
36. tGravityAccMag-std() 
37. tBodyAccJerkMag-mean() 
38. tBodyAccJerkMag-std() 
39. tBodyGyroMag-mean() 
40. tBodyGyroMag-std() 
41. tBodyGyroJerkMag-mean() 
42. tBodyGyroJerkMag-std() 
43. fBodyAcc-mean()-X 
44. fBodyAcc-mean()-Y 
45. fBodyAcc-mean()-Z 
46. fBodyAcc-std()-X 
47. fBodyAcc-std()-Y 
48. fBodyAcc-std()-Z 
49. fBodyAccJerk-mean()-X 
50. fBodyAccJerk-mean()-Y 
51. fBodyAccJerk-mean()-Z 
52. fBodyAccJerk-std()-X 
53. fBodyAccJerk-std()-Y 
54. fBodyAccJerk-std()-Z 
55. fBodyGyro-mean()-X 
56. fBodyGyro-mean()-Y 
57. fBodyGyro-mean()-Z 
58. fBodyGyro-std()-X 
59. fBodyGyro-std()-Y 
60. fBodyGyro-std()-Z 
61. fBodyAccMag-mean() 
62. fBodyAccMag-std() 
63. fBodyBodyAccJerkMag-mean() 
64. fBodyBodyAccJerkMag-std() 
65. fBodyBodyGyroMag-mean() 
66. fBodyBodyGyroMag-std() 
67. fBodyBodyGyroJerkMag-mean() 
68. fBodyBodyGyroJerkMag-std()
