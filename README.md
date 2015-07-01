# R-Cheat-Sheet
- **To load the data from csv file (without headers)**

  >x = read.csv("/path_to_file/file.csv", header = FALSE)

- **To load the data from csv file (without including factors)**

  >x = read.csv("/path_to_file/file.csv", stringsAsFactors = FALSE)

- **To compare two dataframes (cell by cell) and output the result**

  >print(d1==d2)

  * where d1, d2 are dataframes.

  * dimension of two dataframes should be equal

- **To compare two dataframes (cell by cell) and output a summary of the results in tabular form**

  >table(d1==d2)

  * where d1, d2 are dataframes.

  * dimension of two dataframes should be equal

- **To check if a value in a dataframe d1 is present in the same row of a dataframe d2**

  > for(i in 0:n)
  > print(d1[i,] %in% d2[i,])

    * where n is number of rows in dataframe.

    * dimension of two dataframes should be equal.

- **To get the dimension of a dataframe**

  >dim(d1)

- **To get the first or last part of a dataframe**

  >head(d1)
  >tail(d1)

- **To include first n columns in a dataframe(slicing)**

  >d1 = d1[0:n]

- **To count occurence of any specific value in a dataframe d1**

  >length(which(d1=='TRUE'))

- **To sort a dataframe by a specified column or columns **

  >d1 = d1[order(column_name),]

  * default is ASCENDING

  >d1 = d1[order(column_name1, -column_name2),]

  * where d1 is sorted by column_name1 (ascending) and column_name2 (descending)

- **To keep rows with distinct values in column c **

  >d1 = d1[!duplicated(d1$c),]

- **To extract unique elements **

  >v1 = unique(v1)

  * where v1 is a vector

