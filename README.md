
#Cleaning Samsung Galaxy S smartphone data from UCI
##Instructions

###1. Set up
	1. Downloads the 'UCI HAR Dataset' data set and puts the zip file working directory if it doesn't already exist. 
	2. After it is downloaded, it unzips the file into a new UCI HAR Dataset folder.

###2. Load Data and Combine Datasets
	1. load the x datasets for both training and test and combine them by rows. This is taken from the test and train folders.
	2. load the subject datasets for both training and test and combine them by rows. This is taken from the test and train folders.
	3. load the y datasets for both training and test and combine them by rows. This is taken from the test and train folders.

###3. Extract and Label Measurements
	1. Extract the mean and standard deviation columns from the features data set. This is done using grep to identify the keywords.
	2. These column names are then assigned to the x data.
	3. The column names are then formatted.

###4. Assign Activities
	1. Import and format the activity labels from the activity_labels file.
	2. Add the activities to the y data table
	3. Rename the columns for y and subject

###5. Merge and Export
	1. Create a directory for the output files (if one does not already exist).
	2. The three data sets, x, y and subj, are merged. Then, it is exported as a txt file into the Project folder in the same working directory, named merged.txt.
	3. The mean of activities and subjects are created into a separate tidy data set which is exported into the Project folder as txt file; this is named average.txt.

#END