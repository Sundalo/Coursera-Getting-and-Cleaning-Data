#Coursera Data Science: Getting and Cleaning Data Course Project#

The data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained: 

http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones 

The source data for this project can be found here.

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 

#Section 1. Merging the training and the test sets to create one data set.#

After creating the appropriate source directory for the files,  the next step is to read the following into tables:

features.txt
activity_labels.txt
subject_train.txt
x_train.txt
y_train.txt
subject_test.txt
x_test.txt
y_test.txt
Assign column names and merge to create one data set.

#Section 2. Extract only the measurements on the mean and standard deviation for each measurement.#

Create a logcal vector that contains TRUE values for the ID and mean, stdev columns, and FALSE values for the others. Subset this data to keep only the necessary/required columns.

#Section 3. Use descriptions for the  activity names to name the activities in the data set#

Merge data subset with the activityType table to cinlude the descriptive activity names

#Section 4. Properly classify the data set with descriptive activity names.#

Use gsub function for pattern replacement to clean up the data labels.

#Section 5. Create a second, independent tidy data set with the average of each variable for each activity and each subject.#

Per the project instructions, we need to produce only a data set with the average of each veriable for each activity and subject
