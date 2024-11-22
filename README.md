
# Sales Dashboard by Joshua Zireva

A report on sales of cookies sold in united states of America over a period of three years for the years ranging from year 2020 to 2022.

### Data Source
Sales data: The primary dataset used for this project is the "Sales_Data.csv" file containing details of each sale made by the company.

### Tools used
- Power Query to do ETL process
- Power Query to remove unnecessary columns and making some corrections on the data
- Power BI creating reports

### Data Cleaning and preparation 
Initially the following steps were taken:
Data loading and inspection
Remove unnecessary column.
Data cleaning and formatting 
### Exploratory Sales Analysis
What is the overal sales trend?
What are the sales peak periods?
What sales lavel achieved in he same period last year?

```DAX
Calender_Table = CALENDAR(Date(2020,01,01),Date(2022,12,31))
```
### Recommendations

