# WALMART SALES PREDICTION

TIME SERIES ANALYSIS -SARIMA MODEL

## Problem Statement :

A retail store that has multiple outlets across the country are facing issues in managing the inventory - to match the demand with respect to supply. Dataset Information: The walmart.csv contains 6435 rows and 8 columns.

1. You are provided with the weekly sales data for their various outlets. Use statistical analysis, EDA, outlier analysis, and handle the missing values to come up with various insights that can give them a clear perspective on the following:​

a. If the weekly sales are affected by the unemployment rate, if yes - which stores are suffering the most?

​
b. If the weekly sales show a seasonal trend, when and what could be the reason?

c. Does temperature affect the weekly sales in any manner?

​d. How is the Consumer Price index affecting the weekly sales of various stores?

​e. Top performing stores according to the historical data.

​f. The worst performing store, and how significant is the difference between the highest and lowest performing stores.


​### 2. Use predictive modeling techniques to forecast the sales for each store for the next 12 weeks.
Start - Steps Involved

Step 1 - Importing all the required Libraries for Analysis

Step 2 - Importing the walmart Data set through pandas

## Exploratory Data Analysis
step 3 - Extracting the first 20 rows of the Dataset

step 4 - Fetching the unique values from the 'Store' column

step 5 - Fetching the unique values from the 'Holiday_Flag' column

step 6 - Fetching the datatypes information from every columns of the dataset column

step 7 - converting 'object' datatype to 'datetime' datatype

step 8 - finding the null values

step 9 - finding the duplicates values in the data set

## Statistical Analysis
step 10 - getting transposed Statistical summary

step 11 - Analyzing Correlation between the columns

step 12 - droping all columns to the new columns 'col' to run the for loop for Outlier Analysis

## Outlier Analysis
step 13 - Outlier Analysis for every columns through for loop

step 14 - As per the box plot Analysis ,there are outliers present in these columns : Weekly_Sales, Holiday_Flag, Temperature, Unemployment...

## Outlier Removal Technique
step 15 - Lets find out the quantiles and inter-quantile-range and remove the outliers as it is not required for the analysis... #So,lets apply the this technique to remove outlier from the above mentioned columns...

step 16 - Running the loop again to check the outliers:




```bash
  RESULT: -- No oultiers Present after treating it in all the mentioned columns
```


 # Problem Statements : Solutions

## A. If the weekly sales are affected by the unemployment rate, if yes - which stores are suffering the most?

solution : Visualize the relationship between Unemployment Rate and Weekly Sales

![Screenshot (840)](https://github.com/VishnuTejaDumpala/Walmart-Sales-Prediction/assets/170489710/8245bd0d-543c-425b-962d-f414d1faf64e)


```bash
  Correlation between Unemployment Rate and Weekly Sales: -0.10617608965795419.
```

### The store most affected by changes in the unemployment rate is Store 36 Solution : Clearly ,the correlation of columns 'Weekly_Sales' & 'Unemployment' are negative .there is no such dependency between both of them,so 'Unemployment' its not affecting 'Weekly_Sales'

### b. If the weekly sales show a seasonal trend, when and what could be the reason?

![Screenshot (841)](https://github.com/VishnuTejaDumpala/Walmart-Sales-Prediction/assets/170489710/d0a28c6c-2943-42ce-b64b-344f72a9ece7)

![Screenshot (842)](https://github.com/VishnuTejaDumpala/Walmart-Sales-Prediction/assets/170489710/4bb882e8-ac34-45d2-ada2-7a5e175a5242)

![Screenshot (843)](https://github.com/VishnuTejaDumpala/Walmart-Sales-Prediction/assets/170489710/222a7666-29fc-4fc8-8adf-90fc2450fe5a)


### Solution: As per the pattern observed ,weekly sales over time shows seasonal patterns as there are no features variation in the columns

### c. Does temperature affect the weekly sales in any manner?

![Screenshot (830)](https://github.com/VishnuTejaDumpala/Walmart-Sales-Prediction/assets/170489710/58ac6568-65cd-4cc3-83a1-490552a4f3fb)

### Solution :Temperature is not affecting Weekly sales in any way as it is observed from the scatter plot and correlation matrix

D. How is the Consumer Price index affecting the weekly sales of various stores?

![Screenshot (831)](https://github.com/VishnuTejaDumpala/Walmart-Sales-Prediction/assets/170489710/c442d5c7-0dd0-4db8-8de0-36da681f9b81)

e. Top performing stores according to the historical data

![Screenshot (832)](https://github.com/VishnuTejaDumpala/Walmart-Sales-Prediction/assets/170489710/f255c634-d8d4-4ab8-829d-db401269ce99)

![Screenshot (833)](https://github.com/VishnuTejaDumpala/Walmart-Sales-Prediction/assets/170489710/4eb03e83-460c-4dfb-bb93-ce49c45de0a4)

![Screenshot (834)](https://github.com/VishnuTejaDumpala/Walmart-Sales-Prediction/assets/170489710/34bcd362-fb9a-49e8-a9bb-5bbc4aceb560)

## Sales Forecasting using SARIMA Model

### Model Implementation -- Sales Forecast for 12 weeks -- Stores included here are Stores 1,2,3,4,5 (Generating a Forecasts for all 45 stores increases time complexity,hence did it for only 5 stores for evaluation purpose)

![Screenshot (835)](https://github.com/VishnuTejaDumpala/Walmart-Sales-Prediction/assets/170489710/1ff75888-b980-4035-8c00-25e2109c9104)

![Screenshot (836)](https://github.com/VishnuTejaDumpala/Walmart-Sales-Prediction/assets/170489710/01aed36f-5bf9-42e0-83b1-428a01427b6a)

![Screenshot (837)](https://github.com/VishnuTejaDumpala/Walmart-Sales-Prediction/assets/170489710/74ab9821-77c5-4885-a4d1-84b78d65d8e8)

![Screenshot (838)](https://github.com/VishnuTejaDumpala/Walmart-Sales-Prediction/assets/170489710/39eea0c8-f989-4285-8f57-4b7dea677f1e)

![Screenshot (839)](https://github.com/VishnuTejaDumpala/Walmart-Sales-Prediction/assets/170489710/62ea99bb-9911-445b-a54a-2c905de26593)

## END OF THE PREDICTION







