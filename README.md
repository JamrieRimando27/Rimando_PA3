# Programming Assignment 3
#### Deadline: September 10, 2025
## I. Intended Learning Outcomes:
  1. To identify the codes and functions incorporated in the Pandas library
  2. To be able to apply and use the different codes and functions in creating a Python program using a Pandas library
  
## II. Instructions:
  Write a Python script/code in the Jupyter Notebook to do the given problems. You may submit your Jupyter notebook in the dedicated submission bin.

  For this programming assignment, download the following file and save to your default user folder: http://bit.ly/Cars_file
## III. Problems:
  #### 1.) PROBLEM #1: 
  Using knowledge obtained from the experiment and demonstrations:
     
a.) Load the corresponding .csv file into a data frame named cars using pandas
      
b.) Display the first five and last five rows of the resulting cars.
  #### 2.) PROBLEM #2: 
  Using the dataframe cars in problem 1, extract the following information using subsetting, slicing and indexing operations.
    
a.) Display the first five rows with odd-numbered columns (columns 1, 3, 5, 7...) of cars.

b.) Display the row that contains the ‘Model’ of ‘Mazda RX4’.

c.) How many cylinders (‘cyl’) does the car model ‘Camaro Z28’ have?

d.) Determine how many cylinders (‘cyl’) and what gear type (‘gear’) do the car models ‘Mazda RX4 Wag’, ‘Ford Pantera L’ and ‘Honda Civic’ have.
## IV. Answers and Explanation:
### PROBLEM #1
<img width="685" height="720" alt="Image" src="https://github.com/user-attachments/assets/a04a550f-de31-4ef3-ae13-ffa53130c073" />

First, import the pandas library as pd, this library helps in handling data in table form. Then, read a CSV file named "cars.csv" and store its content in a variable called "cars". This file is expected to contain information about different car models . After loading the data, display the first five rows using the "head(5)" function to get a quick look at the beginning of the dataset. Then, display the last five rows using the "tail(5)" function to see the end of the dataset.
### PROBLEM #2
<img width="874" height="792" alt="Image" src="https://github.com/user-attachments/assets/9e401eb6-3612-4169-b2d2-cb394d54aa46" />

Start by importing the pandas library as pd then load a file called "cars.csv" and save the data into a variable named "cars". For problem a, it uses "iloc" to select rows and columns by their positions using numbers. The 0:5 part means it selects the first 5 rows of the data, starting from row 0 up to row 4. The 0::2 part means it picks every second column, starting from the first one. For problem b, a condition "cars['Model'] == 'Mazda RX4'" is used to print the row of Mazda RX4. In problem c, using "loc" to select rows and columns by their positions using names. With the condition "cars['Model'] == 'Camaro Z28'" it will focus only on the row and column of the said model, but it specified "cyl" so it will focus there only. Then ".values[0]" was used to get the get the first element of array, without it, the output will be pandas series. For problem d, filter the dataset to show only specified rows, specifically "Mazda RX4 Wag", "Ford Pantera L", and "Honda Civic". Then, display only specified columns, specifically Model, cyl, gear.
