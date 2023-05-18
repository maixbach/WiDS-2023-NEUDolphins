# WiDS-2023-NEUDolphins: Top 4.4% Global, Top 5 Vietnam
**WiDS 2023 Competition was organized by the WiDS Worldwide team at Stanford University, Harvard University IACS, Arthur, and the WiDS Datathon Committee**

Extreme weather events are sweeping the globe and range from heat waves, wildfires and drought to hurricanes, extreme rainfall and flooding. These weather events have multiple impacts on agriculture, energy, transportation, as well as low resource communities and disaster planning in countries across the globe.

Accurate long-term forecasts of temperature and precipitation are crucial to help people prepare and adapt to these extreme weather events. Currently, purely physics-based models dominate short-term weather forecasting. But these models have a limited forecast horizon. The availability of meteorological data offers an opportunity for data scientists to improve sub-seasonal forecasts by blending physics-based forecasts with machine learning. Sub-seasonal forecasts for weather and climate conditions (lead-times ranging from 15 to more than 45 days) would help communities and industries adapt to the challenges brought on by climate change.

This repository is included models, code and dataset we use in this competition. We reached the position 31/697 teams, at the top 4.4% best results over the globe.


## Dataset
We are using a pre-prepared dataset consisting of weather and climate information for a number of US locations, for a number of start dates for the two-week observation, as well as the forecasted temperature and precipitation from a number of weather forecast models. Each row in the data corresponds to a single location and a single start date for the two-week period. Our task is to predict the arithmetic mean of the maximum and minimum temperature over the next 14 days, for each location and start date.

There are provided with two datasets:

- **train_data.csv**: the training dataset, where contest-tmp2m-14d__tmp2m, the arithmetic mean of the max and min observed temperature over the next 14 days for each location and start date, is provided
- **test_data.csv**: the test dataset, where we withhold the true value of contest-tmp2m-14d__tmp2m for each row.

The  detailed information of variables can be found at: https://www.kaggle.com/competitions/widsdatathon2023/data

## Data Inspection & EDA & Feature Engineering
The detailed processes can be found in our notebook.


## Experimental result
Model         | RMSE
------------- | -------------
Random Forest | 2.304
XGBoost | 1.32
TabNet | 0.984
CatBoost  | 0.98
LightGBM  | 0.907
Ensemble model  | 0.739

## Achievement
With 85 submissions only, our team of 4 reached position 31/697 teams from all over the world, became the top 5 team in Vietnam leaderboard.

