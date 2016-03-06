Experimental design and background

The original data contained a test and train set of an experiment measuring the velocity and gravity of 30 subject on 6 activities.

Firts the variable names of the features.txt data were added to the X-test and X-train files. 
So that all the variable names were more of less descriptive 

Then all the Y_test data was added as a column to the X_test data.
The same was done for the train data. This column were the coded activities and was nemed 'Activity'

Then a column was added from the subject_test data and the subject_train data this Column are the numeric code of the 30 Subjects 
and the column was therfore named 'Subject'.

A column was added for the ACtivity labels : WALKING, SITTING eg (see README).
Then the train and test set were joined together.

Only the measurement with mean and standard deviation measurement were retrieved from the data. And the column names were made 
more descriptive (See also README).

Of these variables a tidy set was made in order to collect the mean of the mean and standard deviation measurements per subject 
and per activity.

