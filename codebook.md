
A full description is available at the site where the data was obtained: 

http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones 

The data for the project: 

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

Training and the test sets were merged:
•test\X_test.txt, test\y_test.txt, test\subject_test.txt were merged into test data table 
•test\X_train.txt, test\y_train.txt, test\subject_train.txt were merged into train data table

From features.txt list of indices corresponding to variables describing mean values and standard deviations. This was done by selecting variables which names contain "mean" or "std". Only the measurements on the mean and standard deviation for each measurement were extracted from both training and test data tables and combined into a single table.

A second data set with the average of each variable for each activity and each subject was created. Each activity label was replaced with corresponding activity name from activity_labels.txt.

The rest of the columns correspond to averaged variables describing mean/std measurements. The names of these variables are same as in features.txt but the values are averages of each variable for each activity and each subject.

The output of the run_analysis.R script is tidydata.txt, also uploaded in the repository.
