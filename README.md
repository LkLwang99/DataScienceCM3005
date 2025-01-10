# CM3005 - Data Science

The project aims to find relationships between the time, interest rate and the price of stock indices whether a linear regression model can find out more about their relationships and use visualizations to project the relationships between time, interest rate and stock indices. 

## 1)Introduction
The project aims to develop a machine learning model that will aid to help us predict the share price of a stock exchange such as NASDAQ if the US's federal reserve interest rate were to increase or decrease with the use of linear regression algorithm.

## 2)Domain-Specific Task and Objectives Of the Project
The Domain-Specific Task is to identify the relationship between the US's federal reserve interest rate and multiple stock exchanges with linear regression.

The impact of the federal reserve interest rate is tremendous on the stock market and signals a great increment or decrement on stock prices. In 2022, when the federal reserve decides to raise the interest rate of the to 3.9%, we could see major stock exchanges had a decline in the prices of the stocks. In 2022, when the federal reserve had announced the increase in interest rate, the S&P 500 as compared to the previous year had fallen which could be seen from the closing price of S&P 500 according to yahoo finance was at Aug 1st 2022 at 4118.63 and Aug 2 2021 at 4422.81 which was a 7% decrease from the previous year. The same scenario is found in the early 2000s, where the federal reserve interest rate rose in the year 2000 and the S&P had fallen by 10.14% but the interest rate began to increase from 4.63% in january 1999 to 6.40% in december 2000.

The contributions which a linear regression machine learning model could help would be to predict the future stock prices if the federal reserve were to decide to raise or lower the interest rates. The machine learning model could help policymakers make better decisions to mitigate the impact of stock market fluctuations on the stock market.

Therefore, the importance of the interest rates to stock prices is justified by historical events and we would want to see if we are able to predict the stock prices increment or decrement based on the interest rates with time series data of the stock prices and the interest rates of the federal reserve with the following objectives:

Gathering the 25-year data of Stock Exchanges And Interest Rate
- Data Cleaning
- Statistical Analysis Of the Data
- Visualisation Of The Data
- Building A Machine Learning Model
- Validation Of the Machine Learning Model
- Feature Engineering
- Evaluation Of the Model


<h2>3)Dataset Description</h2>

<p>For the dataset, the dataset chosen would be the historical stock data prices for several stock index such as Singapore's Straits Time Index, S&P 500 and other major stock indexes. The dataset would be retrieved from the yfinance api which is an open-source and free-to-use api to retrieve data from the yahoo finance. The interest rate would be retrieved from the FRED website with the use of pandas-datareader library as FRED is an accessible database created and maintained by the Research department at Federal Reserve Bank of St. Louis. Therefore, the dataset was collected by making use of the APIs and the pandas_datareader to access the FRED website.
</p>
<br>
<p>The original dataset of the stock indexes collected would be in the following format shown below:

<pre><center>[Date,Open,High,Low,Close,Volume,Dividends,Stocksplits]</center></pre>

The type of the stock indexes retrieved from the yfinance API is in the format where date is shown in datetime format of Year-Month-Date with the hour,minute, seconds and the timezone. The Open,High,Low,Close,Dividends,Stocksplits are
in the format of float and the Volume is in the format of integer. The size of the dataset collected would have 6289 rows and 8 columns which amounts to 50312 data points. </p>
<br>
<p>
Whereas the original dataset of the interest rate collected would be in this format shown below:

<pre><center>[Date, InterestRate]</center></pre>

The type of the date and interest rate retrieved from the FRED website would be displayed as date formatted in Year-Month-Date and the Interest Rate in float. The size of the interest rate dataset which is collected would have 301 rows and 2 columns with the date and interest which amounts to 602 data points as it only consist of interest rate by month.
</p>
<br>
<p>
The final dataset after the preprocessing step to clean out other variables which are not required would be in this format shown below:

<pre><center>[Date,Ticker,interestRate,Price]</center></pre>
</p>
<br>
<p>
An example of the dataset entry would be seen in the example below:

<pre><center>[1999-01-04,GSPC,1229.0,4.63]</center></pre>

From the example displayed, the types of data are shown with date being displayed as year-month-day, the ticker as a string and finally both the interestRate and Price as float. The pre-processing step involves removing unnecessary variables from the stock index dataset and converting the interest from the interest rate dataset from monthly to daily frequency and finally merge the two datasets together as shown in the example before.
</p>
<br>
<p>The size of the final dataset collected and pre-processed should be around 9125 rows of data and 4 columns for both interest rates and stock indexes of different nation which would amount to 36,500 data points.</p>

<center>(432 words)</center>
