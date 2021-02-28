CodeBook 
=================

One new dataset is created by merging the original training and test sets. Only measurements on the mean and standard deviation for each measurement are extracted to creat a smaller dataset. The submitted tidy data set is mainly the averages of each variable of the smaller dataset for each activity and each subject.

The features selected for the original database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. These time domain signals (prefix 't' to denote time) were captured at a constant rate of 50 Hz. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ) using another low pass Butterworth filter with a corner frequency of 0.3 Hz. 

Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag). 

Finally a Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the 'f' to indicate frequency domain signals). 

These signals were used to estimate variables of the feature vector for each pattern:  
'-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.

tBodyAcc-XYZ
tGravityAcc-XYZ
tBodyAccJerk-XYZ
tBodyGyro-XYZ
tBodyGyroJerk-XYZ
tBodyAccMag
tGravityAccMag
tBodyAccJerkMag
tBodyGyroMag
tBodyGyroJerkMag
fBodyAcc-XYZ
fBodyAccJerk-XYZ
fBodyGyro-XYZ
fBodyAccMag
fBodyAccJerkMag
fBodyGyroMag
fBodyGyroJerkMag

In the submitted tidy dataset, the average are only calculated for measurements on the mean and standard deviation of the original dataset: 

mean(): Mean value
std(): Standard deviation

The variables and their units are listed below:

VARIABLE				UNIT
subject				(Subject ID ranging from 1 to 30)
activity				(Classification of activity among LAYING, STADING, 	SITTING, WALKING, WALKING_UPSTAIRS, WALKING DOWNSTAIRS)
tBodyAcc-mean()-X			m/s^2
tBodyAcc-mean()-Y			m/s^2
tBodyAcc-mean()-Z			m/s^2
tBodyAcc-std()-X			m/s^2
tBodyAcc-std()-Y			m/s^2
tBodyAcc-std()-Z			m/s^2
tGravityAcc-mean()-X		m/s^2
tGravityAcc-mean()-Y		m/s^2
tGravityAcc-mean()-Z		m/s^2
tGravityAcc-std()-X			m/s^2
tGravityAcc-std()-Y			m/s^2
tGravityAcc-std()-Z			m/s^2
tBodyAccJerk-mean()-X		m/s^3
tBodyAccJerk-mean()-Y		m/s^3
tBodyAccJerk-mean()-Z		m/s^3
tBodyAccJerk-std()-X			m/s^3
tBodyAccJerk-std()-Y			m/s^3
tBodyAccJerk-std()-Z			m/s^3
tBodyGyro-mean()-X			rad/s
tBodyGyro-mean()-Y			rad/s
tBodyGyro-mean()-Z			rad/s
tBodyGyro-std()-X			rad/s
tBodyGyro-std()-Y			rad/s
tBodyGyro-std()-Z			rad/s
tBodyGyroJerk-mean()-X		rad/s^2
tBodyGyroJerk-mean()-Y		rad/s^2
tBodyGyroJerk-mean()-Z		rad/s^2
tBodyGyroJerk-std()-X		rad/s^2
tBodyGyroJerk-std()-Y		rad/s^2
tBodyGyroJerk-std()-Z		rad/s^2
tBodyAccMag-mean()		m/s^2
tBodyAccMag-std()			m/s^2
tGravityAccMag-mean()		m/s^2
tGravityAccMag-std()		m/s^2
tBodyAccJerkMag-mean()		m/s^3
tBodyAccJerkMag-std()		m/s^3
tBodyGyroMag-mean()		rad/s
tBodyGyroMag-std()			rad/s
tBodyGyroJerkMag-mean()		rad/s^2
tBodyGyroJerkMag-std()		rad/s^2
fBodyAcc-mean()-X			m/s^2
fBodyAcc-mean()-Y			m/s^2
fBodyAcc-mean()-Z			m/s^2
fBodyAcc-std()-X			m/s^2
fBodyAcc-std()-Y			m/s^2
fBodyAcc-std()-Z			m/s^2
fBodyAccJerk-mean()-X		m/s^3
fBodyAccJerk-mean()-Y		m/s^3
fBodyAccJerk-mean()-Z		m/s^3
fBodyAccJerk-std()-X			m/s^3
fBodyAccJerk-std()-Y			m/s^3
fBodyAccJerk-std()-Z			m/s^3
fBodyGyro-mean()-X			rad/s
fBodyGyro-mean()-Y			rad/s
fBodyGyro-mean()-Z			rad/s
fBodyGyro-std()-X			rad/s
fBodyGyro-std()-Y			rad/s
fBodyGyro-std()-Z			rad/s
fBodyAccMag-mean()		m/s^2
fBodyAccMag-std()			m/s^2
fBodyBodyAccJerkMag-mean()		m/s^3
fBodyBodyAccJerkMag-std()		m/s^3
fBodyBodyGyroMag-mean()		rad/s
fBodyBodyGyroMag-std()		rad/s
fBodyBodyGyroJerkMag-mean()	rad/s^2
fBodyBodyGyroJerkMag-std()		rad/s^2

