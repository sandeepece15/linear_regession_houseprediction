# linear_regession_houseprediction# USA Housing Price Prediction using Linear, Ridge, and Lasso Regression

## Project Overview

This project predicts house prices using the **USA Housing** dataset and
compares the performance of three regression algorithms:

-   Linear Regression
-   Ridge Regression
-   Lasso Regression

The project demonstrates the complete machine learning workflow,
including data preprocessing, exploratory data analysis (EDA), model
training, prediction, and evaluation.

------------------------------------------------------------------------

## Dataset

**Dataset:** `USA_Housing.csv`

### Features

-   Avg. Area Income
-   Avg. Area House Age
-   Avg. Area Number of Rooms
-   Avg. Area Number of Bedrooms
-   Area Population

### Target

-   Price

------------------------------------------------------------------------

## Technologies Used

-   Python
-   NumPy
-   Pandas
-   Seaborn
-   Scikit-learn

------------------------------------------------------------------------

## Project Workflow

1.  Import libraries
2.  Load the dataset
3.  Remove the `Address` column
4.  Perform correlation analysis using a heatmap
5.  Split the dataset into training and testing sets
6.  Train the following models:
    -   Linear Regression
    -   Ridge Regression
    -   Lasso Regression
7.  Predict house prices
8.  Evaluate model performance using:
    -   Mean Squared Error (MSE)
    -   R² Score

------------------------------------------------------------------------

## Model Performance

  Model                 Mean Squared Error (MSE)           R² Score
  ------------------- -------------------------- ------------------
  Linear Regression            10,169,125,565.90       0.9185060945
  Lasso Regression         **10,169,124,990.99**   **0.9185060991**
  Ridge Regression             10,169,177,895.81       0.9185056752

------------------------------------------------------------------------

## Results

-   All three models achieved an R² score of approximately **0.9185**,
    indicating that they explain about **91.85%** of the variance in
    house prices.
-   Lasso Regression achieved the lowest MSE and the highest R² score,
    although the improvement over Linear Regression was negligible.
-   Ridge Regression produced nearly identical performance.
-   The results indicate that the dataset already follows a strong
    linear relationship, making regularization less impactful.

