Introduction
The script run_analysis.Rperforms the 5 steps described in the course project's definition.

At the step one, merging x ,y and subject data together  using rbind() function.

In the next step, extracting the rows which only has measures of mean and standard deviation from the merged data. AFter extracting the records, it has been given names which are taken by loading the features.txt
--Then, only those columns with the mean and standard deviation measures are taken from the whole dataset. After extracting these columns, they are given the correct names, taken from features.txt.
As activity data is addressed with values 1:6, we take the activity names and IDs from activity_labels.txt and they are substituted in the dataset.
On the whole dataset, those columns with vague column names are corrected.
Finally, we generate a new dataset with all the average measures for each subject and activity type (30 subjects * 6 activities = 180 rows). The output file is called averages_data.txt, and uploaded to this repository.
