
# Sales Dashboard by Joshua Zireva



### Overview 
This sales dashboard aims to provide insights into the sales performance of a cookie company in United States. By analyzing various aspects of sales data, we seek to identify trends, make data driven recommendations and gain deeper understanding of company's performance. This dashboard is for a period of three years for the years ranging from year 2020 to 2022.



### Data Source
Sales data: The primary dataset used for this project is the "Sales_Data.xlxs" file containing details of each sale made by the company.



### Tools used
- Power Query to do ETL process
- Power Query to remove unnecessary columns and making some corrections on the data
- Power BI creating reports


### Data Cleaning and preparation 
Initially the following steps were taken:
- Data loading and inspection.
- Removing unnecessary column.
- Data cleaning and formatting.

  
### Exploratory Data Analysis

EDA involved exploring the sales data to answer key questions, such as:

- What is the overal sales trend?
- Which state is generating more revenue?
- What sales lavel achieved in the same period last year?


### Data Analysis 


Create a date table
```DAX
Date = ADDCOLUMNS(
    CALENDARAUTO(),
    "Year", YEAR([DATE]),
    "Month", FORMAT([Date], "mmm"),
    "Month Number", Month([Date]),
     "Quarter", FORMAT([Date],"\QQ")
)
```
Some measures:
``` DAX
Revenue Last Year = 
CALCULATE(
    [Total_Revenue],
    SAMEPERIODLASTYEAR('Date'[Date])
)
```


### Results/Findings
Analysis are as follows:

The company sales maintained its upward trajectory in the first year and in august sales dropped and again went up.

Massive sales campaigns are needed in Utah and New York so as to improve sales.



### Recommendations

