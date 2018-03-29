The following transformation were applied to the original data set which can be found here (https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip):
  
Reading "feature.txt" and using it to rename the columns of "X_test.txt"  
Merging relevant objects to get mergedset, mergedlabels & mergedsubject  
Created dataset1 by only extracting variables containing "mean" and "std" from the merged set  

Created dataset2 by aggregating the mean and std for each subject and activity  
Variables  
"mergedsubject" : Subject ID, Integer ranging from 1 to 30  
"mergedlabels": The activity performed by the subject, 6 Factor level:  
* Walking
* Walking_Upstairs
* Walking_Downstairs
* Sitting
* Standing
* Laying  
  
Column 3 to 68: Quantified mean and std features (descripted below) named with the patern [timeSignal|frequencySignal]-[description]-[mean|std] optionnaly followed by .[X|Y|Z]:* mean and std stand for average and standard deviation respectively
