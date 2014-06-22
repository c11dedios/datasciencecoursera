##Getting and cleaning data


###Files in this repository
1. README.md 
2. CodeBook.md 
3. run_analysis.R 

###You should create one R script called run_analysis.R that does the following. 
1. Merges the training and the test sets to create one data set.
2. Extracts only the measurements on the mean and standard deviation for each measurement. 
3. Uses descriptive activity names to name the activities in the data set
4. Appropriately labels the data set with descriptive variable names. 
5. Creates a second, independent tidy data set with the average of each variable for each activity and each subject. 

###It should run in a folder of the Samsung data (the zip had this folder: UCI HAR Dataset) The script assumes it has in it's working directory the following files and folders:

1. activity_labels.txt
2. features.txt
3. test/
4. train/
The output is created in working directory with the name of tidyData.txt


Step by step.

Step 1:
Read all the test and training files: y_test.txt, subject_test.txt and x_test.txt.
Merge the training and the test sets to create one data set.

Step 2:
Read the features from features.txt and leave features that are either means ("mean()") or standard deviations ("std()"). The objective for this step is to only include means and standard deviations of measurements, of which meanFreq() is neither.
A new data frame is then created.

Step 3:
Read the activity names from activity_labels.txt and replace the numbers with the text.

Step 4:
Cleaning up the variable names
Reassigning the new descriptive column names to the finalData set

Step 5:
Create a new data frame using aggregate() function

Final step: Write the new tidy set into a text file called tidyData.txt, formatted similarly to the original files.
