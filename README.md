# R-Cheat-Sheet
- To load the data from csv file (without headers)

  >x = read.csv("/path_to_file/file.csv", header = FALSE)

- To compare two dataframes (cell by cell) and output the result

  >print(d1==d2)

  where d1, d2 are dataframes.


- To check if the value in dataframe d1 is present in the same row of the dataframe d2

  > for(i in 0:38)
  > print(d1[i,] %in% d2[i,])

- To get the dimension of a dataframe

  >dim(d1)
