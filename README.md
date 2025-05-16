# End-To-End-Data-Analytics-Project
Python + SQL
Problem Statement:-We had to download the data set for a company retail orders from kaggle,it conatins the data for the year 2022 and 2023,clean the data set  and provide insights to the stackholder by using SQL. We have followed an ETL process for this particular project.

Extraction Of The Data Set:
We extracted the csv file from the kaggle via an api call made from python and stored it in a data frame
libraries used:-Kagglehub

Exploratory Data Analysis Using Pandas:
During EDA we found out that 
1.One column called 'Ship Mode' had some "not available" values
2.The column names were not in proper format

Data Transformation Using Pandas:
1.Replaced some of the values of 'Ship Mode' with "NA" values.
2.converted the column names to lower case and replaced space with underscore
3.Added new columns like "Discount Price","Sales Price","Profit"
4.Dropped the unnecessary columns
5.Converted the data type of "order_date" to date datatype

Loading the data into MySQL:
After the transformation i loaded the csv file into MYSQL table via python
Libraries Used:sqlalchemy,PyMySQL

Generating Insights in SQL:
After loading the data into MySQl i ran some queries where i have used cte's,case statements,subqueries,group by functons which gave the answers to the below questions:-
1.TOP 10 Products By Revenue
2.TOP 5 Product From Each Region
3.Mom Percentage as compared to last year fo same month
4.For each category which month has the highest sales
5.which sub-category had highest growth by profit in 2023 compared to 2022

