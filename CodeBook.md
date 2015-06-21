Description:

The file tidyDataSet.txt is a processed subset of the original Human Activity Recognition Using Smartphones Data Set produced by UCI Machine Learning repository.
It followed a series of steps including:

- combing the training and the test subjects, activity and reading data files into a single dataset,
- extracting only the measurements corresponding to the mean (Mean) and standard deviation (std) for each available measurement,
- replacing the activities in the data set by descriptive activity names,
- further analysing the mean per each mean (Mean) and standard deviation (std) measurements and sorting by activity and subject.

For more information about how the analysis works, please read README.

Besides grouping by Activity and Subject, the resulting tidy data set contains 66 columns of averaged information (per activity and subject) corresponding to the Mean and standard deviation for the variables in Time and Frequency of magnitude (Mag) and components in X, Y and Z directions for the linear acceleration (Acc), angular acceleration (Gyro), linear jerk (AccJerk) and angular jerk (GyroJerk) for both Body and Gravity components.


The following lines describe each variable, column number, type of data and range of data for the tidy dataset file.

1. Subject

* Subjects that perform a set of activities in the experiment.  [1,30] . Integer values representing a person.

2. Activity

* Activities performed by the test and training subjects. [LAYING, SITTING, STANDING, WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS]. String values representing a activity.

3. Time.BodyAcc.Mean.X

* Average value for the measurements of the Mean of the Body Linear Jerk in the X direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

4. Time.BodyAcc.Mean.Y

* Average value for the measurements of the Mean of the Body Linear Jerk in the Y direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

5. Time.BodyAcc.Mean.Z

* Average value for the measurements of the Mean of the Body Linear Jerk in the Z direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

6. Time.BodyAcc.standardDeviation.X

* Average value for the measurements of the Standard Deviation of the Body Linear Jerk in the X direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

7. Time.BodyAcc.standardDeviation.Y

* Average value for the measurements of the Standard Deviation of the Body Linear Jerk in the Y direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

8. Time.BodyAcc.standardDeviation.Z

* Average value for the measurements of the Standard Deviation of the Body Linear Jerk in the Z direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

9. Time.GravityAcc.Mean.X

* Average value for the measurements of the Mean of the Body Linear Jerk in the X direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

10. Time.GravityAcc.Mean.Y

* Average value for the measurements of the Mean of the Body Linear Jerk in the Y direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

11. Time.GravityAcc.Mean.Z

* Average value for the measurements of the Mean of the Body Linear Jerk in the Z direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

12. Time.GravityAcc.standardDeviation.X

* Average value for the measurements of the Standard Deviation of the Body Linear Jerk in the X direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

13. Time.GravityAcc.standardDeviation.Y

* Average value for the measurements of the Standard Deviation of the Body Linear Jerk in the Y direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

14. Time.GravityAcc.standardDeviation.Z

* Average value for the measurements of the Standard Deviation of the Body Linear Jerk in the Z direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

15. Time.BodyAccJerk.Mean.X

* Average value for the measurements of the Mean of the Body Linear Jerk in the X direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

16. Time.BodyAccJerk.Mean.Y

* Average value for the measurements of the Mean of the Body Linear Jerk in the Y direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

17. Time.BodyAccJerk.Mean.Z

* Average value for the measurements of the Mean of the Body Linear Jerk in the Z direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

18. Time.BodyAccJerk.standardDeviation.X

* Average value for the measurements of the Standard Deviation of the Body Linear Jerk in the X direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

19. Time.BodyAccJerk.standardDeviation.Y

* Average value for the measurements of the Standard Deviation of the Body Linear Jerk in the Y direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

20. Time.BodyAccJerk.standardDeviation.Z

* Average value for the measurements of the Standard Deviation of the Body Linear Jerk in the Z direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

21. Time.BodyGyro.Mean.X

* Average value for the measurements of the Mean of the Body Linear Jerk in the X direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

22. Time.BodyGyro.Mean.Y

* Average value for the measurements of the Mean of the Body Linear Jerk in the Y direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

23. Time.BodyGyro.Mean.Z

* Average value for the measurements of the Mean of the Body Linear Jerk in the Z direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

24. Time.BodyGyro.standardDeviation.X

* Average value for the measurements of the Standard Deviation of the Body Linear Jerk in the X direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

25. Time.BodyGyro.standardDeviation.Y

* Average value for the measurements of the Standard Deviation of the Body Linear Jerk in the Y direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

26. Time.BodyGyro.standardDeviation.Z

* Average value for the measurements of the Standard Deviation of the Body Linear Jerk in the Z direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

27. Time.BodyGyroJerk.Mean.X

* Average value for the measurements of the Mean of the Body Linear Jerk in the X direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

28. Time.BodyGyroJerk.Mean.Y

* Average value for the measurements of the Mean of the Body Linear Jerk in the Y direction in the Time domain for a given Subject doing a specific Activity.  [-1.0,1.0]

29. Time.BodyGyroJerk.Mean.Z

* Average value for the measurements of the Mean of the Body Linear Jerk in the Z direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

30. Time.BodyGyroJerk.standardDeviation.X

* Average value for the measurements of the Standard Deviation of the Body Linear Jerk in the X direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

31. Time.BodyGyroJerk.standardDeviation.Y

* Average value for the measurements of the Standard Deviation of the Body Linear Jerk in the Y direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

32. Time.BodyGyroJerk.standardDeviation.Z

* Average value for the measurements of the Standard Deviation of the Body Linear Jerk in the Z direction in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

33. Time.BodyAccMag.Mean

* Average value for the measurements of the Magnitude of the Mean of the Body Linear Jerk in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

34. Time.BodyAccMag.standardDeviation

* Average value for the measurements of the Magnitude of the Standard Deviation of the Body Linear Jerk in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

35. Time.GravityAccMag.Mean

* Average value for the measurements of the Magnitude of the Mean of the Body Linear Jerk in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

36. Time.GravityAccMag.standardDeviation

* Average value for the measurements of the Magnitude of the Standard Deviation of the Body Linear Jerk in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

37. Time.BodyAccJerkMag.Mean

* Average value for the measurements of the Magnitude of the Mean of the Body Linear Jerk in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

38. Time.BodyAccJerkMag.standardDeviation

* Average value for the measurements of the Magnitude of the Standard Deviation of the Body Linear Jerk in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

39. Time.BodyGyroMag.Mean

* Average value for the measurements of the Magnitude of the Mean of the Body Linear Jerk in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

40. Time.BodyGyroMag.standardDeviation

* Average value for the measurements of the Magnitude of the Standard Deviation of the Body Linear Jerk in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

41. Time.BodyGyroJerkMag.Mean

* Average value for the measurements of the Magnitude of the Mean of the Body Linear Jerk in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

42. Time.BodyGyroJerkMag.standardDeviation

* Average value for the measurements of the Magnitude of the Standard Deviation of the Body Linear Jerk in the Time domain for a given Subject doing a specific Activity. [-1.0,1.0]

43. Frequency.BodyAcc.Mean.X

* Average value for the measurements of the Mean of the Body Linear Jerk in the X direction in the Frequency domain for a given Subject doing a specific Activity. [-1.0,1.0]

44. Frequency.BodyAcc.Mean.Y

* Average value for the measurements of the Mean of the Body Linear Jerk in the Y direction in the Frequency domain for a given Subject doing a specific Activity. [-1.0,1.0]

45. Frequency.BodyAcc.Mean.Z

* Average value for the measurements of the Mean of the Body Linear Jerk in the Z direction in the Frequency domain for a given Subject doing a specific Activity. [-1.0,1.0]

46. Frequency.BodyAcc.standardDeviation.X

* Average value for the measurements of the Standard Deviation of the Body Linear Jerk in the X direction in the Frequency domain for a given Subject doing a specific Activity. [-1.0,1.0]

47. Frequency.BodyAcc.standardDeviation.Y

* Average value for the measurements of the Standard Deviation of the Body Linear Jerk in the Y direction in the Frequency domain for a given Subject doing a specific Activity. [-1.0,1.0]

48. Frequency.BodyAcc.standardDeviation.Z

* Average value for the measurements of the Standard Deviation of the Body Linear Jerk in the Z direction in the Frequency domain for a given Subject doing a specific Activity. [-1.0,1.0]

49. Frequency.BodyAccJerk.Mean.X

* Average value for the measurements of the Mean of the Body Linear Jerk in the X direction in the Frequency domain for a given Subject doing a specific Activity. [-1.0,1.0]

50. Frequency.BodyAccJerk.Mean.Y

* Average value for the measurements of the Mean of the Body Linear Jerk in the Y direction in the Frequency domain for a given Subject doing a specific Activity. [-1.0,1.0]

51. Frequency.BodyAccJerk.Mean.Z

* Average value for the measurements of the Mean of the Body Linear Jerk in the Z direction in the Frequency domain for a given Subject doing a specific Activity. [-1.0,1.0]

52. Frequency.BodyAccJerk.standardDeviation.X

* Average value for the measurements of the Standard Deviation of the Body Linear Jerk in the X direction in the Frequency domain for a given Subject doing a specific Activity. [-1.0,1.0]

53. Frequency.BodyAccJerk.standardDeviation.Y

* Average value for the measurements of the Standard Deviation of the Body Linear Jerk in the Y direction in the Frequency domain for a given Subject doing a specific Activity. [-1.0,1.0]

54. Frequency.BodyAccJerk.standardDeviation.Z

* Average value for the measurements of the Standard Deviation of the Body Linear Jerk in the Z direction in the Frequency domain for a given Subject doing a specific Activity. [-1.0,1.0]

55. Frequency.BodyGyro.Mean.X

* Average value for the measurements of the Mean of the Body Linear Jerk in the X direction in the Frequency domain for a given Subject doing a specific Activity. [-1.0,1.0]

56. Frequency.BodyGyro.Mean.Y

* Average value for the measurements of the Mean of the Body Linear Jerk in the Y direction in the Frequency domain for a given Subject doing a specific Activity. [-1.0,1.0]

57. Frequency.BodyGyro.Mean.Z

* Average value for the measurements of the Mean of the Body Linear Jerk in the Z direction in the Frequency domain for a given Subject doing a specific Activity. [-1.0,1.0]

58. Frequency.BodyGyro.standardDeviation.X

* Average value for the measurements of the Standard Deviation of the Body Linear Jerk in the X direction in the Frequency domain for a given Subject doing a specific Activity. [-1.0,1.0]

59. Frequency.BodyGyro.standardDeviation.Y

* Average value for the measurements of the Standard Deviation of the Body Linear Jerk in the Y direction in the Frequency domain for a given Subject doing a specific Activity. [-1.0,1.0]

60. Frequency.BodyGyro.standardDeviation.Z

* Average value for the measurements of the Standard Deviation of the Body Linear Jerk in the Z direction in the Frequency domain for a given Subject doing a specific Activity. [-1.0,1.0]

61. Frequency.BodyAccMag.Mean

* Average value for the measurements of the Magnitude of the Mean of the Body Linear Jerk in the Frequency domain for a given Subject doing a specific Activity. [-1.0,1.0]

62. Frequency.BodyAccMag.standardDeviation

* Average value for the measurements of the Magnitude of the Standard Deviation of the Body Linear Jerk in the Frequency domain for a given Subject doing a specific Activity. [-1.0,1.0]

63. Frequency.BodyAccJerkMag.Mean

* Average value for the measurements of the Magnitude of the Mean of the Body Linear Jerk in the Frequency domain for a given Subject doing a specific Activity. [-1.0,1.0]

64. Frequency.BodyAccJerkMag.standardDeviation

* Average value for the measurements of the Magnitude of the Standard Deviation of the Body Linear Jerk in the Frequency domain for a given Subject doing a specific Activity. [-1.0,1.0]

65. Frequency.BodyGyroMag.Mean

* Average value for the measurements of the Magnitude of the Mean of the Body Linear Jerk in the Frequency domain for a given Subject doing a specific Activity. [-1.0,1.0]

66. Frequency.BodyGyroMag.standardDeviation

* Average value for the measurements of the Magnitude of the Standard Deviation of the Body Linear Jerk in the Frequency domain for a given Subject doing a specific Activity. [-1.0,1.0]

67. Frequency.BodyGyroJerkMag.Mean

* Average value for the measurements of the Magnitude of the Mean of the Body Linear Jerk in the Frequency domain for a given Subject doing a specific Activity. [-1.0,1.0]

68. Frequency.BodyGyroJerkMag.standardDeviation

* Average value for the measurements of the Magnitude of the Standard Deviation of the Body Linear Jerk in the Frequency domain for a given Subject doing a specific Activity