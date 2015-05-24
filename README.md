

The script run_analysis.R performs the 5 steps described in the course project's definition.

At the step one, merging X_train and X_test into x_data,y_train and y_test into y_data,subject_train and subject_test into subject data using rbind() function.

In the next step, extracting the rows which only has measures of mean and standard deviation from the merged data. After extracting the records, it has been given names which are taken by loading the features.txt

During the third step,since activity data is addressed with values 1:6, we take the activity names and IDs from activity_labels.txt and they are substituted in the dataset.

In Step 4,merge x_data, y_data and subject_data into single whole dataset using cbind() and names are corrected accordingly

Finally, we generate a new dataset with all the average measures for each subject and activity type using ddply() function of plyr package and applying colMeans().  The output file is called averages_data.txt, and uploaded to this repository.

