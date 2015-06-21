 
This github project contains the work to accomplish the project assignment of "Getting and Cleaning Data".
The purpose of this project is to work with, clean a data set so as to be used for later analysis.


# This github main directory includes the following files:

- The raw data files (see sub-directory "UCI_HAR_Dataset", which is required to be placed in your working directory)
- R script ("run_analysis.R") to transform the raw data files into the output ("tidyDataSet.txt"),
which should be downloaded and then read into R with:
read.table("tidyDataSet.txt", header=TRUE)
- A code book ("CodeBook.md") describing each variable and its values in the tidy data set


# How does the script work?

##1  Merges the training and the test sets to create one data set

1.1 clip the training data sets together (activity, subject, reading)
> training <- data.frame()
> training <- cbind(cbind(read.table(file="~/UCI_HAR_Dataset/Train/y_train.txt"), read.table(file="~/UCI_HAR_Dataset/train/subject_train.txt")), read.table(file="~/UCI_HAR_Dataset/train/X_train.txt"))

1.2 clip the test data sets together (activity, subject, reading)
> test <- data.frame()
> test <- cbind(cbind(read.table(file="~/UCI_HAR_Dataset/test/y_test.txt"), read.table(file="~/UCI_HAR_Dataset/test/subject_test.txt")), read.table(file="~/UCI_HAR_Dataset/test/X_test.txt"))

1.3 merge the training and test sets
> step1 <- tbl_df(rbind(training, test))

1.4 set column names to merged set
> colnames(step1) <- c("activity_id", "Subject", as.character(read.table(file="~/UCI_HAR_Dataset/features.txt")[,2]))


##2  Extract only the measurements on the mean and standard deviation

2.1 Select the variables containing mean() and std()
> half_extracted <- step1[, c(grep("activity_id|Subject|mean()|std()", names(step1)))]

2.2 Drop the variables containing meanFreq()
> step2 <- half_extracted[, -c(grep("meanFreq()", names(half_extracted)))]


##3  Replace activity id by descriptive names

3.1 load the activity_labels file
> act_label <- read.table(file="~/UCI_HAR_Dataset/activity_labels.txt")

3.2 add colume names to activity labels set
> colnames(act_label) <- c("activity_id", "Activity")

3.3 add the descriptive names to striped data set
> step2_add_names <- merge(step2, act_label, by = "activity_id")

3.4 drop the activity_id column
> step3 <- select(step2_add_names, -activity_id)


##4  Modify the column names with descriptive names by replacing characters

4.1 Clean up "()-" with "."
> colnames4 <- gsub("\\()-", ".", colnames(step3))

4.2 Remove the suffix "()"
> colnames4 <- gsub("\\()", "", colnames4)

4.3 Elaborate "-mean" with ".Mean"
> colnames4 <- gsub("\\-mean", ".Mean", colnames4)

4.4 Elaborate "-std" with ".standardDeviation"
> colnames4 <- gsub("\\-std", ".standardDeviation", colnames4)

4.5 Elaborate tBody with Time.Body
> colnames4 <- gsub("tBody", "Time.Body", colnames4)

4.6 Elaborate tGravity with Time.Gravity
colnames4 <- gsub("tGravity", "Time.Gravity", colnames4)

4.7 Elaborate fBodyBody with Frequency.Body
> colnames4 <- gsub("fBodyBody", "Frequency.Body", colnames4)

4.8 Elaborate fBody with Frequency.Body
> colnames4 <- gsub("fBody", "Frequency.Body", colnames4)

4.9 Update the colume names of data set
> colnames(step3) <- colnames4


##5 Create a second, independent tidy data set with the average of each variable

5.1 add the prefix "Average." to be in line with the summarized nature of new data set
> step5 <- step3
> colnames5 <- gsub("Time.", "Average.Time.", colnames4)
> colnames5 <- gsub("Frequency.", "Average.Frequency.", colnames5)
> colnames(step5) <- colnames5

5.2 calculate the average of each variable grouping by activity and subject
> step5 <- step5 %>% group_by(Activity, Subject) %>% summarise_each(funs(mean))

5.3 Export the output in the required text file format
> write.table(step5, file="tidyDataSet.txt", sep="\t", row.names=FALSE)
