---
title: "CodeBook.md"
author: "Anuj Parashar"
date: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
output: "final_summarised_dataset.txt"
---
 
## Project Description
The purpose of this project is to demonstrate your ability to collect, work with, and clean a data set. The goal is to prepare tidy data that can be used for later analysis.
 
##Study design and data processing
 
###Collection of the raw data
The original data is already available at the following location:
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 
 
###Notes on the original (raw) data 
For a detailed understanding of how the data is captured and organized, please go through the "README.txt" available with the data (above zip file).
 
##Creating the tidy datafile
 
###Guide to create the tidy data file
* Download the above zip file and extract its content.
* Open the run_analysis.R file and modify the working directory path with the path where you have extracted the above zip file.
* Source the r script, it would create a output file "final_summarised_dataset.txt" in the working directory set in previous step.

###Cleaning of the data
Here are the five steps involved in data cleaning:
* Merges the training and the test sets to create one data set.
* Extracts only the measurements on the mean and standard deviation for each measurement. 
* Uses descriptive activity names to name the activities in the data set
* Appropriately labels the data set with descriptive variable names. 
* From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

For a more detailed description of how this has been acheived in the script, please refer to the readme file at the following location:
https://github.com/promisinganuj/getting-and-cleaning-data/blob/master/README.md

##Description of the variables in the tiny_data.txt file
###Dimensions of the dataset:
'data.frame':	180 obs. of  68 variables

###Summary of the data: 
As mentioned in the step 5 above, this dataset is the average of each variable (feature) for each activity (6 in total) and each subject (30 in total). So, in total there are 30 * 6 observations in this dataset. Also, there are 66 recorded variables for each activity and subject, thats 66 + 2 = 68 columns.

###Variables:
 $ activityId                   : int  1 2 3 4 5 6 1 2 3 4 ...
 
 $ subjectId                    : int  1 1 1 1 1 1 2 2 2 2 ...
 
 $ timeBodyAccMeanX             : num  0.277 0.255 0.289 0.261 0.279 ...
 
 $ timeBodyAccMeanY             : num  -0.01738 -0.02395 -0.00992 -0.00131 -0.01614 ...
 
 $ timeBodyAccMeanZ             : num  -0.1111 -0.0973 -0.1076 -0.1045 -0.1106 ...
 
 $ timeBodyAccStdDevX           : num  -0.284 -0.355 0.03 -0.977 -0.996 ...
 
 $ timeBodyAccStdDevY           : num  0.11446 -0.00232 -0.03194 -0.92262 -0.97319 ...
 
 $ timeBodyAccStdDevZ           : num  -0.26 -0.0195 -0.2304 -0.9396 -0.9798 ...
 
 $ timeGravityAccMeanX          : num  0.935 0.893 0.932 0.832 0.943 ...
 
 $ timeGravityAccMeanY          : num  -0.282 -0.362 -0.267 0.204 -0.273 ...
 
 $ timeGravityAccMeanZ          : num  -0.0681 -0.0754 -0.0621 0.332 0.0135 ...
 
 $ timeGravityAccStdDevX        : num  -0.977 -0.956 -0.951 -0.968 -0.994 ...
 
 $ timeGravityAccStdDevY        : num  -0.971 -0.953 -0.937 -0.936 -0.981 ...
 
 $ timeGravityAccStdDevZ        : num  -0.948 -0.912 -0.896 -0.949 -0.976 ...
 
 $ timeBodyAccJerkMeanX         : num  0.074 0.1014 0.0542 0.0775 0.0754 ...
 
 $ timeBodyAccJerkMeanY         : num  0.028272 0.019486 0.02965 -0.000619 0.007976 ...
 
 $ timeBodyAccJerkMeanZ         : num  -0.00417 -0.04556 -0.01097 -0.00337 -0.00369 ...
 
 $ timeBodyAccJerkStdDevX       : num  -0.1136 -0.4468 -0.0123 -0.9864 -0.9946 ...
 
 $ timeBodyAccJerkStdDevY       : num  0.067 -0.378 -0.102 -0.981 -0.986 ...
 
 $ timeBodyAccJerkStdDevZ       : num  -0.503 -0.707 -0.346 -0.988 -0.992 ...
 
 $ timeBodyGyroMeanX            : num  -0.0418 0.0505 -0.0351 -0.0454 -0.024 ...
 
 $ timeBodyGyroMeanY            : num  -0.0695 -0.1662 -0.0909 -0.0919 -0.0594 ...
 
 $ timeBodyGyroMeanZ            : num  0.0849 0.0584 0.0901 0.0629 0.0748 ...
 
 $ timeBodyGyroStdDevX          : num  -0.474 -0.545 -0.458 -0.977 -0.987 ...
 
 $ timeBodyGyroStdDevY          : num  -0.05461 0.00411 -0.12635 -0.96647 -0.98773 ...
 
 $ timeBodyGyroStdDevZ          : num  -0.344 -0.507 -0.125 -0.941 -0.981 ...
 
 $ timeBodyGyroJerkMeanX        : num  -0.09 -0.1222 -0.074 -0.0937 -0.0996 ...
 
 $ timeBodyGyroJerkMeanY        : num  -0.0398 -0.0421 -0.044 -0.0402 -0.0441 ...
 
 $ timeBodyGyroJerkMeanZ        : num  -0.0461 -0.0407 -0.027 -0.0467 -0.049 ...
 
 $ timeBodyGyroJerkStdDevX      : num  -0.207 -0.615 -0.487 -0.992 -0.993 ...
 
 $ timeBodyGyroJerkStdDevY      : num  -0.304 -0.602 -0.239 -0.99 -0.995 ...
 
 $ timeBodyGyroJerkStdDevZ      : num  -0.404 -0.606 -0.269 -0.988 -0.992 ...
 
 $ timeBodyAccMagMean           : num  -0.137 -0.1299 0.0272 -0.9485 -0.9843 ...
 
 $ timeBodyAccMagStdDev         : num  -0.2197 -0.325 0.0199 -0.9271 -0.9819 ...
 
 $ timeGravityAccMagMean        : num  -0.137 -0.1299 0.0272 -0.9485 -0.9843 ...
 
 $ timeGravityAccMagStdDev      : num  -0.2197 -0.325 0.0199 -0.9271 -0.9819 ...
 
 $ timeBodyAccJerkMagMean       : num  -0.1414 -0.4665 -0.0894 -0.9874 -0.9924 ...
 
 $ timeBodyAccJerkMagStdDev     : num  -0.0745 -0.479 -0.0258 -0.9841 -0.9931 ...
 
 $ timeBodyGyroMagMean          : num  -0.161 -0.1267 -0.0757 -0.9309 -0.9765 ...
 
 $ timeBodyGyroMagStdDev        : num  -0.187 -0.149 -0.226 -0.935 -0.979 ...
 
 $ timeBodyGyroJerkMagMean      : num  -0.299 -0.595 -0.295 -0.992 -0.995 ...
 
 $ timeBodyGyroJerkMagStdDev    : num  -0.325 -0.649 -0.307 -0.988 -0.995 ...
 
 $ freqBodyAccMeanX             : num  -0.2028 -0.4043 0.0382 -0.9796 -0.9952 ...
 
 $ freqBodyAccMeanY             : num  0.08971 -0.19098 0.00155 -0.94408 -0.97707 ...
 
 $ freqBodyAccMeanZ             : num  -0.332 -0.433 -0.226 -0.959 -0.985 ...
 
 $ freqBodyAccStdDevX           : num  -0.3191 -0.3374 0.0243 -0.9764 -0.996 ...
 
 $ freqBodyAccStdDevY           : num  0.056 0.0218 -0.113 -0.9173 -0.9723 ...
 
 $ freqBodyAccStdDevZ           : num  -0.28 0.086 -0.298 -0.934 -0.978 ...
 
 $ freqBodyAccJerkMeanX         : num  -0.1705 -0.4799 -0.0277 -0.9866 -0.9946 ...
 
 $ freqBodyAccJerkMeanY         : num  -0.0352 -0.4134 -0.1287 -0.9816 -0.9854 ...
 
 $ freqBodyAccJerkMeanZ         : num  -0.469 -0.685 -0.288 -0.986 -0.991 ...
 
 $ freqBodyAccJerkStdDevX       : num  -0.1336 -0.4619 -0.0863 -0.9875 -0.9951 ...
 
 $ freqBodyAccJerkStdDevY       : num  0.107 -0.382 -0.135 -0.983 -0.987 ...
 
 $ freqBodyAccJerkStdDevZ       : num  -0.535 -0.726 -0.402 -0.988 -0.992 ...
 
 $ freqBodyGyroMeanX            : num  -0.339 -0.493 -0.352 -0.976 -0.986 ...
 
 $ freqBodyGyroMeanY            : num  -0.1031 -0.3195 -0.0557 -0.9758 -0.989 ...
 
 $ freqBodyGyroMeanZ            : num  -0.2559 -0.4536 -0.0319 -0.9513 -0.9808 ...
 
 $ freqBodyGyroStdDevX          : num  -0.517 -0.566 -0.495 -0.978 -0.987 ...
 
 $ freqBodyGyroStdDevY          : num  -0.0335 0.1515 -0.1814 -0.9623 -0.9871 ...
 
 $ freqBodyGyroStdDevZ          : num  -0.437 -0.572 -0.238 -0.944 -0.982 ...
 
 $ freqBodyAccMagMean           : num  -0.1286 -0.3524 0.0966 -0.9478 -0.9854 ...
 
 $ freqBodyAccMagStdDev         : num  -0.398 -0.416 -0.187 -0.928 -0.982 ...
 
 $ freqBodyBodyAccJerkMagMean   : num  -0.0571 -0.4427 0.0262 -0.9853 -0.9925 ...
 
 $ freqBodyBodyAccJerkMagStdDev : num  -0.103 -0.533 -0.104 -0.982 -0.993 ...
 
 $ freqBodyBodyGyroMagMean      : num  -0.199 -0.326 -0.186 -0.958 -0.985 ...
 
 $ freqBodyBodyGyroMagStdDev    : num  -0.321 -0.183 -0.398 -0.932 -0.978 ...
 
 $ freqBodyBodyGyroJerkMagMean  : num  -0.319 -0.635 -0.282 -0.99 -0.995 ...
 
 $ freqBodyBodyGyroJerkMagStdDev: num  -0.382 -0.694 -0.392 -0.987 -0.995 ...

###activityId
* The activity performed by the subjects.
* Six Unique values: 1 WALKING, 2 WALKING_UPSTAIRS, 3 WALKING_DOWNSTAIRS, 4 SITTING, 5 STANDING, 6 LAYING
* Unit: NA

###subjectId
* The id of the volunteers who performed these activities.
* Thirty Unique values: 1 - 30
* Unit: NA

###Rest of the variable are average values for each subject and each activity.
* Each variable is abbreviated using the following meanings:

  time: Time domain signal

  freq: Frequence domain signal

  BodyAcc: Body acceleration signals

  GravityAcc: Gravity acceleration signals

  Gyro: Gyroscope reading

  Jerk: Jerk Signal

  Mag: Magnitude

  Mean: Mean value

  StdDev: Standard Deviation
