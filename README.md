# Bike-Sharing-Demand-Prediction
## Project Type - Regression
## Contribution - Individual
## Team Member - Nandini K S
## Project Summary

1. Data Collection:

Importing libraries

Dataset Loading

About the dataset

2. Data Cleaning:

Finding Duplicate values

Finding Missing/Null values

Understanding your variables

Handling Outliers

3. Data Wrangling and Feature Engineering

4. Exploratory Data Analysis(EDA):

Univariate Analysis

Bivariate Analysis

5. Data Preprocessing:

Checking distribution of each feature and trensform it to normal distribution

Checking relationship between independent and dependent variables is linear

Checking multicollinearity in independent variables

Features encoding

Data Splitting

Data Scaling

6. Supervise Machine learning algorithms and implementation:

Linear Regression

Lasso Regression

Ridge Regression

ElasticNet Regression

Decision Tree

Random Forest

XGBoost

7.Model Evaluation

8. Model Explainability

## Problem Statement
Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes.

## Data Description
The dataset contains weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall), the number of bikes rented per hour and date information.

Attribute Information:

Date : year-month-day

Rented Bike count - Count of bikes rented at each hour

Hour - Hour of the day

Temperature-Temperature in Celsius

Humidity - %

Windspeed - m/s

Visibility - 10m

Dew point temperature - Celsius

Solar radiation - MJ/m2

Rainfall - mm

Snowfall - cm

Seasons - Winter, Spring, Summer, Autumn

Holiday - Holiday/No holiday

Functional Day - NoFunc(Non Functional Hours), Fun(Functional hours)

## Let's Begin !
## Exploratory data analysis
### Univariate Analysis
Observations :

Customers equally favour renting motorcycles in all seasons.

Customers choose to rent motorcycles when there are no holidays. They rarely use the bikes while traveling on vacation.

Nearly all consumers preferred to rent bikes during functional hours.

Bicycle rentals are popular throughout the month.

Renting bicycles was not very popular in 2017, but it increased by 83.02 percent in 2018.



### Bivariate Analysis

## 1. Plotting graph of Rented Bike Count by hour

Customers do not prefer to use rented bikes at night.

Customers do not prefer rented bikes in the early mornings hours of 4 and 5, but the usage increases from 7, 8, and 9, possibly due to people commuting to work. The same trend is observed in the evenings of 5, 6, and 7, as people travel from the work to home. Overall, the rented bike was the most frequently used during office commute times.

Customers mostly use rented bikes for transportation in the evening.


## 2.Effect of temperature(°C) on rented bike usage
Observations :

Customers prefer to use rented bikes when the temperature is normal, but they do not use them when the temperature is below normal.

### 3. Effect of each variable on the usage of rented bikes
Obsevations :

Customers who travel most commonly use rented bikes in the morning at 8 a.m. and in the evening at 6 p.m.

People prefer to rent bikes when the humidity level is between 10% and 18%.

Customers consistently use rented bikes when the wind speed is between 2 m/s and 3.5 m/s, and usage is at its highest when the wind speed is normal, which is 3.2 m/s.

Renting a bike is the best option for customers when the dew point temperature ranges from 12°C to 18°C. Usage of rented bikes increases with increasing dew point temperatures, but it still peaks at normal dew point temperatures.

According to the graph, solar radiation has no effect on customer use of rented bikes.

People prefer to rent bikes the most when it is not raining.

When there is no snowfall, most people choose to rent bikes. However, the majority of customers prefer to rent bikes when it snows up to 4 cm.

In the first 10 days of the month, most rented bikes are used by customers. Customers consistently use rented bikes in the last 15 days of the month.

June has the highest usage of rented bikes throughout the year, followed by October. Customers usage of rented bikes is at its peak from April to September.

### 4. Effect of visibility on Rented bike count
Observation :

The count of rented bikes on that day is unaffected by the day's visibility, but when visibility exceeds 1750, use of rented bikes increases more than usual.

### 5. Bar graph of (Seasons, Holiday, Fuctioning Day, Year) VS Rented Bike Count
Observations :

Most people rent bikes during the summer and autumn seasons. Fewer people choose to rent bikes during the winter.

People rent bikes even when there is no holiday, and usage on non-holiday days is higher than on holidays.

Almost every rented bike is used during its functional hours.

The use of rented bikes increased by three times in 2018 compared to 2017.


# Conclusion

Customers equally prefer renting motorcycles in all seasons.

Customers choose to rent motorcycles when there are no holidays. They rarely use the bikes they rent while traveling on vacation.

Nearly all consumers prefer to rent bikes during functional hours.

Bicycle rentals are popular throughout the month.

Renting bicycles was not very popular in 2017, but it increased by 83.02 percent in 2018.

Customers do not prefer to use rented bikes at night.

Customers do not prefer rented bikes in the early mornings hours of 4 and 5, but uasage increases from 7, 8, and 9, possibly due to people commuting to work. The same trend is observed in the evenings 5, 6, and 7, as people travel from work to home. Overall, the rented bike was the most frequently used during office commute times.

Customers mostly use rented bikes for transportation in the evening.

Customers who travel most commonly use rented bikes in the morning at 8 a.m. and in the evening at 6 p.m.

Customers prefer to rent bikes When the humidity level is between 10% and 18%.

Customers consistently use rented bikes when the wind speed is between 2 m/s and 3.5 m/s, and usage is at its highest when wind speed is normal, which is 3.2 m/s.

Renting a bike is the best option for customers when the dew point temperature ranges from 12°C to 18°C. Usage of rented bike increases with increases with increasing dew point temperatures, but it still peaks at normal dew point temperatures.

According to the graph, solar radiation has no effect on customer use of rented bikes.

People prefer to rent bikes the most when it is not raining.

When there is no snowfall, most people choose to rent bikes. However, the majority of customers prefer to rent bikes when it snows up to 4 cm.

In the first 10 days of the month, most rented bikes are used by customers. Customers consistently use rented bikes in the last 15 days of the month.

June has the highest usage of rented bikes throughout the year, followed by October. Customers usage of rent bikes is at its peak from April to September.

The count of rented bikes on a day is not affected by the day's visibility. However, when visibility exceeds 1750, use of rented bikes increases more than usual.

Most people rent bikes during the summer and autumn seasons, while fewer people choose to rent bikes during the winter.

People rent bikes even when there is no holiday, and usage on non-holiday days is higher than on holiday.

Almost every rented bike is used during its functional hours.

The use of rented bikes increased by three times in 2018 compared to 2017.

The XGBoost regression model has the highest R-squared score, the lowest Root Mean Squared Error (RMSE), and has mean of residuals that are very close to zero.

Therefore, due to the model's high accuracy, low error, and near-zero mean of residuals, the XGBoost regression model is the ideal and well-trained model for forecasting the number of rented bikes required per hour.

