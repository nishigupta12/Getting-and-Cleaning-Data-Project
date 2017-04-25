## Code Book For Tidy Data Set (course project)
This code book describes the variables in the tidy data set (TidySet.txt).  The analysis steps are in the README.md file.

### Variable 1
Variable 1 (in column 1) = subject:  subject number of test volunteer, ranging from 1 to 30. Each of the 30 volunteers performed 6 activities wearing a smartphone (Samsung Galaxy S II).

### Variable 2
Variable 2 (in column 2) = activity: type of activity performed during the test.  The data is ordered in the activity sequence listed below. The type # refers to the number in the source files but is not listed in this column to improve readability (e.g., it is descriptive).
* WALKING (activity type #1)
* WALKING_UPSTAIRS (activity type #2)
* WALKING_DOWNSTAIRS (activity type #3)
* SITTING (activity type #4)
* STANDING (activity type #5)
* LAYING (activity type #6)

There is 1 set of observations per volunteer and activity combination (180 rows).

### Background On Observations In Original Source Files
The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. These time domain signals (prefix 't' to denote time) were captured at a constant rate of 50 Hz. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ) using another low pass Butterworth filter with a corner frequency of 0.3 Hz. 

Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag). 

Finally a Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the 'f' to indicate frequency domain signals). 

These signals were used to estimate variables of the feature vector for each pattern:  
'-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.

* tBodyAcc-XYZ
* tGravityAcc-XYZ
* tBodyAccJerk-XYZ
* tBodyGyro-XYZ
* tBodyGyroJerk-XYZ
* tBodyAccMag
* tGravityAccMag
* tBodyAccJerkMag
* tBodyGyroMag
* tBodyGyroJerkMag
* fBodyAcc-XYZ
* fBodyAccJerk-XYZ
* fBodyGyro-XYZ
* fBodyAccMag
* fBodyAccJerkMag
* fBodyGyroMag
* fBodyGyroJerkMag


### Tidy Data Set:  Subset of Observation Variables
This is a subset of the total original observations.  It includes all the variables where "mean", "Mean", or "std"" (standard deviation) show up in the variable name.

* mean(): Mean value
* std(): Standard deviation
* meanFreq(): Weighted average of the frequency components to obtain a mean frequency

Additional vectors obtained by averaging the signals in a signal window sample. These are used on the angle() variable:

* gravityMean
* tBodyAccMean
* tBodyAccJerkMean
* tBodyGyroMean
* tBodyGyroJerkMean

###  Tidy Data Set: Variable Names
Variables 3 - 81 (columns 3 - 81) = These are the subset of variables that include mean and std in their names.  The colummn names were simplified to make them more descriptive.  The - and () were removed and first letters of mean and std were capitalized for consistency.

3. tBodyAccMeanX
4. tBodyAccMeanY
5. tBodyAccMeanZ
6. tBodyAccStdX
7. tBodyAccStdY
8. tBodyAccStdZ
9. tGravityAccMeanX
10. tGravityAccMeanY
11. tGravityAccMeanZ
12. tGravityAccStdX
13. tGravityAccStdY
14. tGravityAccStdZ
15. tBodyAccJerkMeanX
16. tBodyAccJerkMeanY
17. tBodyAccJerkMeanZ
18. tBodyAccJerkStdX
19. tBodyAccJerkStdY
20. tBodyAccJerkStdZ
21. tBodyGyroMeanX
22. tBodyGyroMeanY
23. tBodyGyroMeanZ
24. tBodyGyroStdX
25. tBodyGyroStdY
26. tBodyGyroStdZ
27. tBodyGyroJerkMeanX
28. tBodyGyroJerkMeanY
29. tBodyGyroJerkMeanZ
30. tBodyGyroJerkStdX
31. tBodyGyroJerkStdY
32. tBodyGyroJerkStdZ
33. tBodyAccMagMean
34. tBodyAccMagStd
35. tGravityAccMagMean
36. tGravityAccMagStd
37. tBodyAccJerkMagMean
38. tBodyAccJerkMagStd
39. tBodyGyroMagMean
40. tBodyGyroMagStd
41. tBodyGyroJerkMagMean
42. tBodyGyroJerkMagStd
43. fBodyAccMeanX
44. fBodyAccMeanY
45. fBodyAccMeanZ
46. fBodyAccStdX
47. fBodyAccStdY
48. fBodyAccStdZ
49. fBodyAccMeanFreqX
50. fBodyAccMeanFreqY
51. fBodyAccMeanFreqZ
52. fBodyAccJerkMeanX
53. fBodyAccJerkMeanY
54. fBodyAccJerkMeanZ
55. fBodyAccJerkStdX
56. fBodyAccJerkStdY
57. fBodyAccJerkStdZ
58. fBodyAccJerkMeanFreqX
59. fBodyAccJerkMeanFreqY
60. fBodyAccJerkMeanFreqZ
61. fBodyGyroMeanX
62. fBodyGyroMeanY
63. fBodyGyroMeanZ
64. fBodyGyroStdX
65. fBodyGyroStdY
66. fBodyGyroStdZ
67. fBodyGyroMeanFreqX
68. fBodyGyroMeanFreqY
69. fBodyGyroMeanFreqZ
70. fBodyAccMagMean
71. fBodyAccMagStd
72. fBodyAccMagMeanFreq
73. fBodyBodyAccJerkMagMean
74. fBodyBodyAccJerkMagStd
75. fBodyBodyAccJerkMagMeanFreq
76. fBodyBodyGyroMagMean
77. fBodyBodyGyroMagStd
78. fBodyBodyGyroMagMeanFreq
79. fBodyBodyGyroJerkMagMean
80. fBodyBodyGyroJerkMagStd
81. fBodyBodyGyroJerkMagMeanFreq
