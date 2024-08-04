# Gold Price Prediction

This project focuses on predicting gold prices using machine learning techniques. The model utilizes a Random Forest Regressor to achieve high accuracy in predicting gold prices based on historical data.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Data Description](#data-description)
3. [Data Preprocessing](#data-preprocessing)
4. [Exploratory Data Analysis](#exploratory-data-analysis)
5. [Model Training](#model-training)
6. [Model Evaluation](#model-evaluation)
7. [Results Visualization](#results-visualization)
8. [Conclusion](#conclusion)

## Project Overview
The goal of this project is to predict the price of gold using historical data. We employ a Random Forest Regressor, a powerful ensemble learning method, to achieve a high R-squared value, indicating the model's accuracy in explaining the variance in gold prices.

## Data Description
The dataset used in this project is stored in `gld_price_data.csv` and contains the following columns:
- `Date`: Date of the record
- `SPX`: S&P 500 index value
- `GLD`: Gold price
- `USO`: Crude oil price
- `SLV`: Silver price
- `EUR/USD`: Euro to USD exchange rate

## Data Preprocessing
1. Load the dataset using Pandas.
2. Inspect the first and last few rows of the dataset to understand its structure.
3. Check the number of rows and columns.
4. Obtain basic information about the data, including data types and non-null counts.
5. Check for missing values.
6. Generate statistical measures of the data.

## Exploratory Data Analysis
1. Compute the correlation matrix to understand the relationships between features.
2. Visualize the correlation matrix using a heatmap.
3. Analyze the distribution of the gold price using a distribution plot.

## Model Training
1. Split the data into features (`X`) and target (`Y`), where `X` contains all columns except `Date` and `GLD`, and `Y` contains the `GLD` column.
2. Further split the data into training and testing sets using an 80-20 split.
3. Train a Random Forest Regressor with 100 estimators on the training data.

## Model Evaluation
1. Predict gold prices on the test data.
2. Compare the predicted values with the actual values.
3. Calculate the R-squared error to evaluate the model's performance. An R-squared value of 0.98 indicates that the model explains 98% of the variance in gold prices.

## Results Visualization
1. Plot the actual vs. predicted gold prices to visually assess the model's performance.
2. Use a line plot to show the comparison between actual and predicted values.

## Conclusion
The Random Forest Regressor model demonstrates a high accuracy in predicting gold prices, with an R-squared value of 0.98. This indicates that the model effectively captures the underlying patterns in the data, making it a reliable tool for gold price prediction.

