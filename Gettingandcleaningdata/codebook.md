##Getting and cleaning data

Data: 
The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. These time domain signals (prefix 't' to denote time) were captured at a constant rate of 50 Hz. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ) using another low pass Butterworth filter with a corner frequency of 0.3 Hz. 

Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag). 

Finally a Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the 'f' to indicate frequency domain signals). 

These signals were used to estimate variables of the feature vector for each pattern:  
'-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.


subject    

    subjectID              Unique identifier assigned to each subject

label                      activityType

1. "WALKING
2. "WALKING_UPSTAIRS"
3. "WALKING_DOWNSTAIRS"
4. "SITTING"
5. "STANDING"
6. "LAYING"

The signals are:

1.  tBodyAcc-XYZ
2.  tGravityAcc-XYZ
3.  tBodyAccJerk-XYZ
4.  tBodyGyro-XYZ
5.  tBodyGyroJerk-XYZ
6.  tBodyAccMag
7.  tGravityAccMag
8.  tBodyAccJerkMag
9.  tBodyGyroMag
10. tBodyGyroJerkMag
11. fBodyAcc-XYZ
12. fBodyAccJerk-XYZ
13. fBodyGyro-XYZ
14. fBodyAccMag
15. fBodyAccJerkMag
16. fBodyGyroMag
17. fBodyGyroJerkMag


The set of variables that were estimated from these signals are:

1. mean(): Mean value
2. std(): Standard deviation





