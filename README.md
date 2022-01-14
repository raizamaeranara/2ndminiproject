Name: Raiza Mae Ranara

Course & Year: BS in Statistics III

Section: 3
_____________________________________________________________________________________

Problem 1

  Download the zipped file UCI_HAR_Dataset.zip from the LMS. Unzip the file and create a directory ‘specdata’ in your local file. 
  DO NOT make any modifications in the files included in the zipped file. The data set is about Human Activity Recognition Using Smartphones. 
  The data includes were collected from the accelerometers from the Samsung Galaxy S smartphone. 
  You can check the full description of the dataset from http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones. 


  a.	Create an R script called run_analysis.R. The script should include the following: 

      •	Merges the training and the test sets to create one data set. 
      
      •	Extracts only the measurements on the mean and standard deviation for each measurement 
      
      •	Uses descriptive activity names to name the activities in the dataset 
      
      •	Appropriately labels the data set with descriptive variable names 
      
      •	From the data set in step 4, create a second, independent tidy data set with the average of each variable for each activity and each subject.


_____________________________________________________________________________________
  •	Step 1: Merges the training and the test sets to create one data set with target variables.
  
      o	Read all the test and training files: X_test.txt , y_test.txt, and subject_test.txt.
      
      o	Combine the files to a data frame in the form of subjects, labels, the rest of the data.
      
  •	Step 2: Extracts only the measurements on the mean and standard deviation for each measurement.
  
      o	Read the features from features.txt and filter it to only leave features that are either means ("mean()") or standard deviations ("std()"). 
      
      o	A new data frame is then created that includes subjects, labels, and the described features.
      
  •	Step 3: Uses descriptive activity names to name the activities in the data set.
  
      o	Read the activity labels from activity_labels.txt and replace the numbers with the text.
      
  •	Step 4: Appropriately labels the data set with target variables with descriptive names.
  
      o	Make a column list
      
      o	Tidy the list by removing all non-alphanumeric characters and converting the result to lowercase 
      
      o	Apply the column names to the data frame
      
  •	Step 5: From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.
  
      o	Create a new data frame by finding the mean for each combination of subject and label. 

