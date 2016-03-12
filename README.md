# fitness_data_analysis
Analyzes smart phone fitness data from: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip contains all the data and readme files used 
in conducting an experiment by the researchers.

The analysis I performed took the data files, comprised of the raw data, user ID's, and activities, combined both test and training 
data files into a single data set, and then summarized them. Below is a sample of the first ten rows of data. 
subject_id activity                                variable        mean
1           1  WALKING    Time Domain Signal of BodyAcc-mean-X  0.27733076
2           1  WALKING    Time Domain Signal of BodyAcc-mean-Y -0.01738382
3           1  WALKING    Time Domain Signal of BodyAcc-mean-Z -0.11114810
4           1  WALKING     Time Domain Signal of BodyAcc-std-X -0.28374026
5           1  WALKING     Time Domain Signal of BodyAcc-std-Y  0.11446134
6           1  WALKING     Time Domain Signal of BodyAcc-std-Z -0.26002790
7           1  WALKING Time Domain Signal of GravityAcc-mean-X  0.93522320
8           1  WALKING Time Domain Signal of GravityAcc-mean-Y -0.28216502
9           1  WALKING Time Domain Signal of GravityAcc-mean-Z -0.06810286
10          1  WALKING  Time Domain Signal of GravityAcc-std-X -0.97660964

The purpose of the task was to combine the subject_id, experiment participant in this case, with the activity, and the time or frequency data gathered from the smartphone. The smartphone collected X, Y, and Z coordinates of the participants' movements. Next,
I presented only the mean and standarard deviation of the X, Y, and Z components of the time and frequency data. This analysis includes mean and standard deviation and omits many of the other variables such as mad, min, max, energy, iqr, entropy, and so on. Whereas the original data contained 561 factor level variables, this analysis contains only 86. The combined test and training data contains 15,480 observations.

In the features.txt file, the file list 561 variables with names such as "tBodyAcc-mean()-X" or "fBodyAcc-mean()-X." I replaced this terminology, t or f, with "Time Domain Signal" and "Fast Fourier Transform" for better readability. I left the "X", "Y", and "Z" coordinates since these are potentially meaningful.



