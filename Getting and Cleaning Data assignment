##assignment
#You should create one R script called run_analysis.R that does the following.

##Merges the training and the test sets to create one data set.
##Extracts only the measurements on the mean and standard deviation for each measurement.
##Uses descriptive activity names to name the activities in the data set
##Appropriately labels the data set with descriptive variable names.
##From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

## to read the data


install.packages("plyr")
library(plyr)

install.packages("base")
library(base)

install.packages("sqldf")
library(sqldf)


setwd("E:/Kennis/Coursera/Data scientist Getting and cleaning data/UCI HAR Dataset/")

subject_train <-read.table("train/subject_train.txt")
subject_test <-read.table("test/subject_test.txt")

X_train <-read.table("train/X_train.txt")
X_test <-read.table("test/X_test.txt")

Y_train <-read.table("train/Y_train.txt")
Y_test <-read.table("test/Y_test.txt")

activity_labels <-read.table("activity_labels.txt")
features <-read.table("features.txt")

##############
##Combine subject_train to the measurement data
##Combine subject_test to the measurement data

## I have done things not in the same order but the result is the same

## Add the variables to the X-test and X-train data from the features data
names(X_test)<- features$V2
names(X_train)<- features$V2
## Add new column activity to test and train set

X_test1 <-cbind(Y_test,X_test)
X_train1 <-cbind(Y_train,X_train)

# change the new column name to activity
names(X_test1)[1] <- "Activity"
names(X_train1)[1] <- "Activity"

# Add new column subject to the test and train set
X_test2 <-cbind(subject_test,X_test1)
X_train2 <-cbind(subject_train,X_train1)

# change the new column name to subject
names(X_test2)[1] <- "Subject"
names(X_train2)[1] <- "Subject"

# Combine the train and test set
X_test_train <-rbind(X_train2,X_test2)

#Change the name of the column in activity label
names(activity_labels)[1] <- "Activity"
names(activity_labels)[2] <- "Activity_label"


#################################
##join the two tabel so that the activity labels are available
Total_data_set <- join(X_test_train, activity_labels, type="left",match="all")

#################################
##To select only the mean and standard deviation first
## selection of all the names that contain mean or std
subsetfeatures<-features$V2[grep("mean\\(\\)|std\\(\\)", features$V2)]

## Make a data frame that makes in possible to select the right columns in de total data set
selected_columns<-c("Subject", "Activity", "Activity_label", as.character(subsetfeatures))
## select only the columns we want namly only the ones that have mean and std and the rest of the necessary columns
Mean_std<-subset(Total_data_set,select=selected_columns)

#####################################################
## Change the variable names to the variables: according to features info t=time and f=frequency. 
##I presume I have to changes these names to the full name.

## to lookup all the columns names in this case (plus three extra columns)
selected_columns

##Change the names of all the column names
names(Mean_std)<-gsub("^t", "MEANoftime", names(Mean_std))
names(Mean_std)<-gsub("^f", "MEANoffrequency", names(Mean_std))

names(Mean_std)<-gsub("Acc", "Accelerometer", names(Mean_std))
names(Mean_std)<-gsub("Gyro", "Gyroscope", names(Mean_std))
names(Mean_std)<-gsub("Mag", "Magnitude", names(Mean_std))
names(Mean_std)<-gsub("BodyBody", "Body", names(Mean_std))
names(Mean_std)<-gsub("-mean()", "mean", names(Mean_std))
names(Mean_std)<-gsub("-std", "Standaardeviation", names(Mean_std))


#########################################
##Tidy data
##to group_by the data
Tidy_data<-aggregate(. ~Subject + Activity_label, Mean_std, mean)
## to order the data by SUbject and Activity (because this is numeric)
Tidy_data<-Tidy_data[order(Tidy_data$"Subject",Tidy_data$"Activity"),]
## create a table
write.table(Tidy_data, file = "tidydata.txt",row.name=FALSE)

#########################################
str(Tidy_data)
summary(Tidy_data)
