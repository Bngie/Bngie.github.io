# 1. Wages Index and CPI

### 1) Get the data

- Average Weekly Earnings of Alberta

[Economic Dashboard - Average Weekly Earnings](https://economicdashboard.alberta.ca/AverageWeeklyEarnings)

Download the data with xlsx. format.

![1%20Wages%20Index%20and%20CPI%209411e189c6d648f3bf48d8a118cdc84f/Untitled.png](1%20Wages%20Index%20and%20CPI%209411e189c6d648f3bf48d8a118cdc84f/Untitled.png)

I chose 'When' column and 'Alberta' column for the average weekly earnings. 

Since I'm only interested in 2011~2021 data, use filter function in excel to choose the date range. 

- CPI of Alberta

[Economic Dashboard - Consumer Price Index Change](https://economicdashboard.alberta.ca/ConsumerPriceIndexChange#alberta)

![1%20Wages%20Index%20and%20CPI%209411e189c6d648f3bf48d8a118cdc84f/Untitled%201.png](1%20Wages%20Index%20and%20CPI%209411e189c6d648f3bf48d8a118cdc84f/Untitled%201.png)

Similarly, I filtered out 2011 ~ 2021 data and chose only 'All-items' in 'Commodity' column. So I got a reference date and Alberta's CPI. 

- Let's copy and paste the selected columns in a new workbook. And change the column name. (Make sure to align columns in the same starting row to match the date.)

![1%20Wages%20Index%20and%20CPI%209411e189c6d648f3bf48d8a118cdc84f/Untitled%202.png](1%20Wages%20Index%20and%20CPI%209411e189c6d648f3bf48d8a118cdc84f/Untitled%202.png)

### 2) Formatting

- Change the format for 'Weekly Earnings' column to currency with a single decimal point.
- Change the format for 'Date' column to short date and delete one of the 'Date' columns.
- Change the format for 'CPI' column to number.

There is an notion in Excel because the number is saved with the text format. We can fix this with **Split texts to Columns** function.

![1%20Wages%20Index%20and%20CPI%209411e189c6d648f3bf48d8a118cdc84f/Untitled%203.png](1%20Wages%20Index%20and%20CPI%209411e189c6d648f3bf48d8a118cdc84f/Untitled%203.png)

![1%20Wages%20Index%20and%20CPI%209411e189c6d648f3bf48d8a118cdc84f/Untitled%204.png](1%20Wages%20Index%20and%20CPI%209411e189c6d648f3bf48d8a118cdc84f/Untitled%204.png)

- Finally, Aligning to the middle. Now we have a clean data to analyze.

![1%20Wages%20Index%20and%20CPI%209411e189c6d648f3bf48d8a118cdc84f/Untitled%205.png](1%20Wages%20Index%20and%20CPI%209411e189c6d648f3bf48d8a118cdc84f/Untitled%205.png)

### 3) Wages Index

- To make Weekly Earnings to Index, let's set 2011-01-01 wages as a base. Insert a new column and name it as 'Wages Index' and create a formula by selecting the first row of the 'Weekly Earnings' column and divide it by the same cell(base). Make sure to let the base as an absolute reference(F4). Lastly multiply 100 with a bracket.

![1%20Wages%20Index%20and%20CPI%209411e189c6d648f3bf48d8a118cdc84f/Untitled%206.png](1%20Wages%20Index%20and%20CPI%209411e189c6d648f3bf48d8a118cdc84f/Untitled%206.png)

### 4) Analysis

- To compare the trend in wages index and CPI, create a line chart. Select the 'Date', 'Wages Index', 'CPI' columns and insert a line chart.
- To see a clear view of the comparison, increase the minimum of y-axis as 80 and select the unit for 10.

![1%20Wages%20Index%20and%20CPI%209411e189c6d648f3bf48d8a118cdc84f/Untitled%207.png](1%20Wages%20Index%20and%20CPI%209411e189c6d648f3bf48d8a118cdc84f/Untitled%207.png)

We can see that between 2014-2018, there is ups and downs for Wages Index. So the CPI increased more than wages over that time. Also, from 2020-2021, we can see that there is a jump in wages index which might indicate the reflection of job losses related to COVID-19 being concentrated among lower-paid employees.