# Bike-Rental-count

## 1.Project Summary:
Bike sharing system is an innovative transportation strategy that provides individuals with bikes for their common use on a short-term basis for a price or for free. Over the last few decades, there has been a significant increase in the popularity of bike-sharing systems all over the world. This is because it is an environmentally sustainable, convenient and economical way of improving urban mobility. In addition to this, this system also helps to promote healthier habits among its users and reduce fuel consumption.

---
![Bike-Sharing-Demand-1194x501](https://user-images.githubusercontent.com/63404689/230723473-74a6a130-2eb3-49e8-8bb7-108658f19582.jpg)
---

## 2. Problem Description
Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes.

## 3. Data Description
The dataset contains weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall), the number of bikes rented per hour and date information.
Attribute Information:
Date : year-month-day
Rented Bike count - Count of bikes rented at each hour
Hour - Hour of he day
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
Building a Regression Model

## 4. Methodology:
We first build several individual regression models such as Linear, Ridge, Random Forest, Gradient Boost and Adaboost. We then use 'Stacking' approach where the predictions from these level 1 individual models are used as meta-features to build a second level model (Linear Regressor, Random Forest and Gradient Boost) to further enhance the predicting capabilities.

## 5. Colclusion
The key takeaway from the EDA and Modeling are
- Bike rental count is strongly correlated with the time of the day, with weaker dependence on the temperature and humidity
There are 2 rental patterns across the day in bike rentals count
- First on a Working Day where the rental count high at peak office hours (8am and 5pm) and
- Second on a Non-working day where rental count is more or less uniform across the day with a peak at around noon.

Below figure shows the bike rental behavior and our model predictions on the test set data for a Random Forest Model

## 6. Tool Used
- Pandas

![Pandas_logo](https://user-images.githubusercontent.com/63404689/230723284-ce30ea90-1ac6-4c82-b227-5364e12fd292.png)

- NumPy

![NumPy_logo](https://user-images.githubusercontent.com/63404689/230723166-4514ab2c-48dc-4ada-b4ca-93aa1bd9b030.png)

- Matplotlib

![logo2](https://user-images.githubusercontent.com/63404689/230723363-c4f64e3e-d834-42d6-8bdc-230642e809ec.svg)

- Seaborn

![seaborn](https://user-images.githubusercontent.com/63404689/230723386-0e1a1fea-2219-42b8-9e76-51ed6e6107dc.png)

- Scikit-Learn

![1200px-Scikit_learn_logo_small svg](https://user-images.githubusercontent.com/63404689/230723495-8d98bb54-e52d-4f59-9887-251344f18a2a.png)


