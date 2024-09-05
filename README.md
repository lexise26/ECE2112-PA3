# ECE2112-PA3
## EXPERIMENT 3: PYTHON DATA ANALYSIS (PANDAS)

### Custodio, Louise Angela G.
## 2ECE-D

**I. Intended Learning Outcomes**:
1. To identify the codes and functions incorporated in the Pandas library.
2. To be able to apply and use the different codes and functions in creating a Python program using a Pandas library.

**II. Instructions:**
Write a Python script/code in the Jupyter Notebook to do the given problems. You may submit your Jupyter notebook in the dedicated submission bin.

## Problems
**PROBLEM 1:** Using knowledge obtained from the experiment and demonstrations:

a. Load the corresponding .csv file into a data frame named cars using pandas

b. Display the first five and last five rows of the resulting cars.


**PROBLEM 2:** Using the dataframe cars in problem 1, extract the following information using subsetting, slicing and
indexing operations.

a. Display the first five rows with odd-numbered columns (columns 1, 3, 5, 7...) of cars.

b. Display the row that contains the ‘Model’ of ‘Mazda RX4’.

c. How many cylinders (‘cyl’) does the car model ‘Camaro Z28’ have?

d. Determine how many cylinders (‘cyl’) and what gear type (‘gear’) do the car models ‘Mazda RX4
Wag’, ‘Ford Pantera L’ and ‘Honda Civic’ have.


## How I did my code:

### **PROBLEM 1**

![PA3-1 1](https://github.com/user-attachments/assets/23697162-9d78-4067-87f7-a9210861339f)
![PA3-1 2 (2)](https://github.com/user-attachments/assets/9ef5d6aa-288a-4be8-8bd8-aa688d46021a)

Step 1: Import the Pandas Library - I began by importing the pandas library to load and manipulate the datase which is the ‘import pandas as pd’. This is a necessary step to utilize the ‘read_csv’ function, which reads CSV files into pandas DataFrames.

Step 2:  Load the CSV File into a DataFrame - Using the ‘pd.read_csv()’ function, I loaded the 'cars.csv' file into a pandas DataFrame named cars. This function reads the contents of the CSV file and stores the data in a structured tabular format.

Step 3: Display the First Five Rows - To view the first five rows of the dataset, I used the 'cars.head(5)' method. This is useful to quickly view the top entries of the DataFrame and ensure that the data was loaded correctly.

Step 4: Display the Last Five Rows - To view the last five rows of the dataset, I used the 'cars.tail(5)' method. This helps verify the structure of the dataset by viewing the bottom rows, ensuring the data has been correctly read.



### **PROBLEM 2**

![PA3-2 1](https://github.com/user-attachments/assets/7df97cea-9a23-4029-98f2-d10ff3494e1e)
![PA3-2 2](https://github.com/user-attachments/assets/435bfc5e-7987-4de0-8b6b-07441fa78e74)
![PA3-2 3 (2)](https://github.com/user-attachments/assets/b9e5b363-5ac9-46e5-9b19-a6f16cab0ba6)

Step 1: Assign DataFrame to a Variable - I assigned the DataFrame cars from Problem 1 to a new variable c to simplify referencing it in further operations.

Step 2: Display the First Five Rows with Odd-Numbered Columns - To display the first five rows and select only the odd-numbered columns (1, 3, 5, 7...), I used the ‘.iloc[]’ function. The first argument [0,1,2,3,4] selects the first five rows, and the second argument [1,3,5,7,9,11] selects the odd-numbered columns based on their index positions (starting from 0).

Step 3: Display the Row for the Car Model 'Mazda RX4' - I used the ‘.loc[]’ function to find the row where the 'Model' column has the value 'Mazda RX4'. This returns all the details for the row matching that condition.

Step 4: Find the Number of Cylinders ('cyl') for the Car Model 'Camaro Z28' - I filtered the DataFrame using ‘.loc[]’ to find the 'Model' 'Camaro Z28'. I then selected only the 'Model' and 'cyl' columns to display how many cylinders the Camaro Z28 has.

Step 5: Determine Cylinders ('cyl') and Gear Type ('gear') for Specific Car Models - I used the ‘.loc[]’ function to filter the rows for the models 'Mazda RX4 Wag', 'Ford Pantera L', and 'Honda Civic' by combining conditions with the | (OR) operator. I then selected the 'Model', 'cyl', and 'gear' columns to display the relevant information.

## Conclusion

This experiment offered valuable insights into the practical use of pandas for data manipulation and analysis. It involved loading data from a CSV file into a pandas DataFrame and employing various functions to inspect and manage the dataset. Key skills developed include using methods such as `.head()`, `.tail()`, and `.iloc[]` for viewing and indexing data. Additionally, the experiment demonstrated how to use `.loc[]` for filtering data to retrieve specific rows and columns based on set conditions. This hands-on experience showcased the efficiency of these pandas functions in managing and analyzing real-world data, making data exploration and extraction of meaningful insights more effective.
