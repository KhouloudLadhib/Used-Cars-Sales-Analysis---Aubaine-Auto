# Aubaine Auto 2024 Sales Analysis

## I. Goal
This python code analyzes data of used cars sold in 2024 in the car dealer Aubaine Auto to identify any patterns in sales. In other words, the goal is to identify, if there are, any ways to increase used cars sales for Aubaine Auto through investing in new sales channels, buying specific car models, focusing on older or newer models, etc. Below are the questions that the project answers.

* How much does a car spend in stock on average before being sold? (for KPI purposes)
* Which car brands/models does Aubaine auto buy and sell the most?
* Do older cars sell faster or slower than newer cars?
* Are there more successful sales channels than others? (for investment purposes)
* Are there months where cars sell much more than others? (for preparing inventory)
* Do cheaper cars sell faster or slower than more expensive cars?
* Do cars sell faster when they are discounted?

## II. Data
The dataset was collected by the salesman of Aubaine Auto, Khalil Daoues, and myself. The data consists 113 lines. Each line corresponds to a car that is eiher sold in 2024 or bought in 2024 and not sold yet.
There are 25 rows in the dataset.

### 1. Descriptive Data
* CAR
* BRAND
* MODEL_NAME
* MODEL_YEAR
* VIN (Vehicle Identification Number)
* PRICE_INITIAL
* PRICE_FINAL (Price at which the car was sold)

### 2. Sales Channels
* MARKETP.
* AUTO\nHEBDO
* CARGURUS
* DRIVE\nGOOD
* SALE_CHANNEL (Sales Channel through which the car was sold)

### 3. Timeline
* PURCH_DATE
* PURCH_DAY
* PURCH_MONTH
* PURCH_YEAR
* SALE_DATE
* SALE_DAY
* SALE_MONTH
* SALE_YEAR
* Days_Brand (Average number of days in stock for the brand of the car)
* Days_Model (Average number of days in stock for the model of the car)
* Days_Year_Make (Average number of days in stock for the year of make of the car)
* Days_Initial_Price (Average number of days in stock for the price of the car)

## III. Summary of Analysis
Firstly, the data was prepared by removing rows of unsold cars since they are irrelevent for this study. Then, missing data were replaced. Some of the questions were answered by simply making a calculation. Others required scatter plots, a bar plot, a pie chart and a line graph. For creating the graphs, the analysis mostly used the groupby() function paired with count(), sum(), std() or mean(). In addition, a two-tailed t-test was performed to test for significant difference between two means.



## IV. Conclusion and Recommendation

The results show that on average, a used car spends 94 days in stock at Aubaine Auto. This should be checked against similar small used car dealers to see if this number is low or high. Mitsubishi and Hyundai are the cars that are bought and sold the most with Mitsubishi RVR being the top model. There doesn't seem to be a relationship between the year in which the cars were made and the number of days they stay in stock. June and November were the months with the highest number of sold cars while July and September were the months with the lowest number of sales. However, July can be considered an outlier since, according to the car dealer, the salesman was on vacation that month.
Facebook marketplace, Khalil and walk-ins account for 2/3rds of sales. It is important to note that only a few cars were posted on the cars websites and therefore we cannot say that these websites are not successful in selling the Aubaine Auto cars. We recommend posting all cars in all channels in 2025 to be able to identify which channels are worth investing on in future years. The days spent in stock by discounted cars is significantly higher than the days spent in stock by non discounted cars. This does not necessarily mean causation. We recommend collecting data of when the discount was made to determine if cars stay in stock longer because they are discounted or they are disconted because they stayed in stock too long. Cheaper cars seem to be selling faster than more expensive cars.
