The original dataset is downloaded with the given url and the download function from the downloader package. Since .zip is a kind of binary file, "mode = 'wb' " should be added to the download function. The downloaded .zip file is then unzipped.

After checking the .txt files from the downloaded dataset, I find that the data are stored as tables of numbers separated with single spaces, so I choose to use read.tables to read the data.

The number of rows of the data in 'subject_test', 'y_test' and 'X_test' are the same, so is the case with 'subject_train', 'y_train' and 'X_train'. After quick check using the table function, it's obvious that the data in 'subject_*' are subject IDs (7 subjects in the test set and 21 in the traing set, which sums 30 in total), and the data in 'y_*' are activity index ranging from 1-6. So these said 6 dataframes are merged into one big dataframe.

Column names of the new merged dataset is updated according to features.txt. Then columns with names only with 'mean()' and 'std()' are selected out according to instruction No.2.

Activity classification are changed from number of 1-6 to concrete names according to the mapping in activity_labels.txt.

The select data are checked and there wad no NA.

In the end, the selected data are grouped with 30 different subject IDs and 6 kinds of activity and then averaged by 30*6=180 groups. 