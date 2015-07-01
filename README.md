# R-Cheat-Sheet
- To load the data from csv file (without headers)

  >x = read.csv("/path_to_file/file.csv", header = FALSE)

- To compare two dataframes (cell by cell) and output the result

  >print(d1==d2)

  where d1, d2 are dataframes.

  dimension of two dataframes should be equal


- To check if a value in a dataframe d1 is present in the same row of a dataframe d2

  > for(i in 0:n)
  > print(d1[i,] %in% d2[i,])

    where n is number of rows in dataframe.

    dimension of two dataframes should be equal.

- To get the dimension of a dataframe

  >dim(d1)
