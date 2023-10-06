# Airplane-Data-Analysis-Project

Created this amazing project with a report to present the findings. To create this project used a few libraries such as Pandas, Matplotlib, Seaborn, and Sqlite3 for using the SQL commands. The dataset is taken from the Kaggle website the link for the dataset is: https://www.kaggle.com/datasets/fiazbhk/airline-data-analysis

## The Questions used to solve this dataset are:
1. How many planes have more than 100 seats?
2. How do the number of tickets booked and the total amount earned change with time?
3. Calculate the average charges for each aircraft with different fare conditions
4. For each aircraft, calculate the total revenue per year and the average return per ticket.
5. Calculate the average occupancy per aircraft.
6. Calculate by how much the total annual turnover could increase by giving all aircraft a 10% higher occupancy rate.

## To perform the analysis, I've used Jupyter Notebook
First, I created a database connection to import the file, to do that I used the "sqlite3.connect" function to form a connection to the data file, using the ‘. execute' function I retrieved all the values into a variable for better analysis.

## Data Exploration
After importing all the values into variables, I explored the data to look into the table to identify the data for analysis and to solve the problems.

## Data Cleaning
After exploration, I tried to clean the data to remove any missing values or to fill any missing values present in the dataset.

## Analysis
Question 1. How many planes have more than 100 seats?

To solve this question, I used the ‘. read_sql_query' function from pandas to select the files from the dataset to calculate the values of seats.
  
Question 2. How the number of tickets booked and the total amount earned change with time?
 
To solve this question, I used the ‘. read_sql_query' function from pandas to select the files from the dataset and I also used the '.to_datetime' function to convert the values of a particular column to date time format, by creating a separate column for it and calculated the tickets booked on what time, used line and bar graph to represent the findings.
  
Question 3. Calculate the average charges for each aircraft with different fare conditions

To solve this question, I used the ‘. read_sql_query' function from pandas to select the files from the dataset and I used the "Seaborn" library to graph a bar chart to represent the finding. 
  
Question 4. For each aircraft, calculate the total revenue per year and the average return per ticket.

To solve this question, I used the ‘. read_sql_query' function from pandas to select the files from the dataset and I used the 'join' function from SQL to join two tables to get the total_revenue and average_revenue respectively.
  
Question 5. Calculate the average occupancy per aircraft.

To solve this question, I used the ‘. read_sql_query' function from pandas to select the files from the dataset and I used the 'inner join' function from SQL to join two tables to get the occupancy_rate of the airline for each aircraft to calculate which airplane has the max occupancy rate.
  
Question 6. Calculate by how much the total annual turnover could increase by giving all aircraft a 10% higher occupancy rate.

To solve this question, I used the ‘. read_sql_query' function from pandas to select the files from the dataset used the 'join' function from SQL to join two tables to get the total_revenue and total_annual_turnover, and used the ‘. set_option' function to convert the float values to string values for better visualization purposes.

And I also created a report explaining the details of this analysis.
