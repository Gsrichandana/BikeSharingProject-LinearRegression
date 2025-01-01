# BIKE SHARING PROJECT
> This project involves building a multiple linear regression model to predict the demand for shared bikes based on various independent variables. The dataset is provided by BoomBikes, a bike-sharing company that aims to forecast the demand for bikes after the pandemic, using factors such as weather, season, time of the year, and other relevant data.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
Background of the Project:

BoomBikes, a bike-sharing company, operates a system where bikes are made available to individuals for short-term use, either for free or for a fee. The company has faced significant challenges due to the COVID-19 pandemic, which drastically affected the demand for shared bikes. As the world slowly recovers from the pandemic and markets begin to stabilize, BoomBikes aims to understand the factors that drive bike rental demand in order to create an effective business plan for the post-pandemic market.

BoomBikes seeks to use data-driven insights to forecast bike demand, optimize bike distribution, improve fleet management, and adjust business strategies to cater to consumer needs as the market reopens. By building a predictive model, BoomBikes intends to understand the dynamics of bike rentals and identify key variables influencing demand.

Business Problem:

The business problem that this project addresses is how to predict the demand for shared bikes (total number of bike rentals) based on several independent factors. This will help BoomBikes optimize bike availability, make informed marketing decisions, and manage fleet resources more efficiently.

The model will allow BoomBikes to:

Forecast bike rental demand on specific days.
Identify the impact of external factors like weather conditions, season, and time of the year on bike demand.
Adjust business operations according to predicted demand (e.g., ensuring enough bikes are available during peak demand periods).
Dataset:

The dataset used for this project contains daily data about bike rentals, along with several associated features such as weather, season, time of the year, and other meteorological information. Specifically, the dataset includes:

Target Variable: cnt (Total bike rentals on a given day, combining both casual and registered users).
Independent Variables:
season: Categorical variable indicating the season (1=Spring, 2=Summer, 3=Fall, 4=Winter).
weathersit: Categorical variable indicating the weather condition (1=Clear, 2=Partly cloudy, 3=Cloudy, 4=Rain).
temp, atemp: Numeric variables indicating the temperature and "feels-like" temperature, respectively.
humidity: Percentage of humidity in the air.
windspeed: Wind speed on a given day.
hour, weekday, month, year: Temporal features related to the time of day, day of the week, month, and year.
casual and registered: Number of rentals by casual users and registered users, respectively.
The dataset is designed to model bike rental demand as influenced by weather conditions, time of year, and other external factors. The target variable (cnt) combines the number of rentals from both casual and registered users, making it the central focus for prediction.

Project Objective:

The primary objective of this project is to build a multiple linear regression model that can predict bike rental demand (cnt) based on various independent features. This model will help BoomBikes understand how factors like weather conditions, seasonality, and temporal data (time of the year, day of the week) impact bike demand, and will assist the company in better planning for fleet management and resource allocation in the future.
<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
Conclusion 1: Seasonality Plays a Significant Role in Bike Demand

The analysis of the dataset reveals that seasonal factors significantly impact the demand for shared bikes. For instance, bike rentals are generally higher during the spring and summer seasons (seasons 1 and 2), and lower during the fall and winter seasons (seasons 3 and 4). The positive correlation between seasonality and bike demand suggests that warmer weather encourages more people to rent bikes, while colder weather and harsher conditions (like rain or snow) decrease demand. Therefore, understanding and accounting for seasonal variations is crucial for predicting bike demand and making adjustments to fleet availability.

Conclusion 2: Weather Conditions Influence Bike Rentals

Weather conditions such as wind speed are also significant predictors of bike rental demand. From the model, it is evident that:
Wind speed may discourage bike rentals, as strong winds tend to reduce outdoor activities.
Thus, BoomBikes can use weather forecasts to adjust operations, ensuring that bikes are available during favorable weather conditions, while reducing fleet size or adjusting business strategies on days with unfavorable weather.

Conclusion 3: The Year (yr) Variable is Important

Even though the yr variable (indicating the year: 0 for 2018 and 1 for 2019) initially appears as a trivial factor, it proves to be an important predictor. The analysis suggests that there was a steady increase in bike rentals from 2018 to 2019, possibly due to growing awareness of bike-sharing systems and the expansion of the company's operations. Dropping this variable could lead to loss of valuable information, as it captures trends and growth in the business. The model benefits from including the yr variable to track changes in demand over time, which can be useful for future forecasts.
<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
NumPy - Version: 1.23.1
Used for numerical operations, working with arrays, and performing mathematical functions.
Pandas - Version: 1.4.2
Used for data manipulation, cleaning, and processing, particularly for handling the dataset and performing data wrangling tasks.
Matplotlib - Version: 3.5.2
Used for data visualization, particularly for plotting graphs and charts like histograms, scatter plots, and line plots to explore the dataset.
Seaborn - Version: 0.11.2
Built on top of Matplotlib, Seaborn is used for more advanced data visualizations with an emphasis on statistical plotting, such as heatmaps for correlation matrices and pair plots.
Scikit-learn - Version: 1.1.1
A library for machine learning that provides tools for data preprocessing, model building, splitting datasets, scaling data, and evaluating models using metrics like R-squared.
Statsmodels - Version: 0.13.2
Used for performing Multiple Linear Regression and statistical tests, as well as calculating variance inflation factors (VIF) for multicollinearity diagnostics.
Scikit-learn's MinMaxScaler - Version: 1.1.1
Used for scaling continuous features to a range (0, 1), which helps in ensuring that all features are treated on the same scale.
Scikit-learn's r2_score - Version: 1.1.1
Used for evaluating the performance of the regression model, specifically calculating the R-squared value to measure the goodness of fit.

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project is part of the IIIB masters project.

## Contact
Created by [@Gsrichandana] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->