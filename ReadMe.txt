README

This repository contains

1. The R script to actually test the R Code. 
2. A Codebook to describe the step by step process of getting and cleaning the data
3. And this read me text file.

The final output of dataset combines the test and training data. Then the column was further selected
to have the mean and standard deviation measures only. Furthermore, there is a requirement to provide
an independent dataset that computes the average of each variable by grouping the activities

Steps in achieving the results
1. I imported the relevant libraries
2. Then I focus on the dataset that will achieve the requirements
	> The X and Y train - the data and the key rows
	> The X and Y test - the data and the key rows
	> the features - for the column names
	> the activity labels - for the description of the activities
3. Clean the features vector
	> cleaning it by removing the open and close parenthesis 
	> changing the data type 
	> removing the "," instead replacing it with a "-"
4. After cleaning the features, I attach the features as column name for both test and train
5. Then I add the key rows by using "cbind"
6. Then I extracted the activity labels to further join them with the key rows to achieve a descriptive rows
7. Then I extracted the column name that has an activity description and keys with "GREPL" function to extract the measures that has 'mean' and 'std'
8. Finally I created a independent tidy data set that groups the data with their activity labels with each data point is an average


https://github.com/TravisJohn/GettingAndCleaningData