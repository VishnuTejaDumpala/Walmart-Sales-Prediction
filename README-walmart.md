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

​

### 2. Use predictive modeling techniques to forecast the sales for each store for the next 12 weeks.
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

 