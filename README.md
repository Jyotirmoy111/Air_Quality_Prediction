# Air_Quality_Prediction

Project Overview

Air quality prediction is an essential task to understand and mitigate the impact of air pollution on human health and the environment. This Python project aims to build a machine learning model that can predict air quality based on historical air quality data. The project involves data preprocessing, exploratory data analysis, feature selection, model training, evaluation, and visualization of results.

Project Goals

Data Preprocessing: Clean and preprocess the air quality dataset to handle missing values and ensure data quality.
Exploratory Data Analysis (EDA): Understand the underlying patterns and relationships in the data through visualization and statistical analysis.
Feature Selection: Identify the most relevant features that contribute to air quality prediction.
Model Training: Train machine learning models, including linear regression and regularized regression techniques like Lasso regression, to predict air quality.
Model Evaluation: Evaluate the performance of the models using metrics such as Mean Squared Error (MSE) and R-squared (R²) score.
Visualization: Visualize the actual vs. predicted air quality values and the correlation between different features.

Dataset

The dataset used in this project is the "AirQualityUCI.csv" file, which contains hourly averaged responses from an array of 5 metal oxide chemical sensors embedded in an Air Quality Chemical Multisensor Device. The dataset includes various air quality-related parameters, such as CO, NMHC, NOx, and NO2 concentrations, as well as meteorological data.

Steps Involved

1. Data Loading and Inspection
Load the dataset using Pandas.
Inspect the first few rows and summary statistics to understand the data structure.

2. Data Preprocessing
Replace missing values (-200 in the dataset) with NaN.
Drop non-numeric columns, such as date and time, which are not useful for regression modeling.
Use SimpleImputer to replace missing values with the mean of each column.
Standardize the features using StandardScaler.

3. Exploratory Data Analysis (EDA)
Plot histograms and box plots to visualize the distribution of features.
Create a correlation heatmap to identify relationships between features.

4. Feature Selection
Select relevant features for the prediction task.
Define the target variable (CO(GT) in this case).

5. Model Training
Split the dataset into training and testing sets using train_test_split.
Train a Linear Regression model and a Lasso Regression model.
Use cross-validation to tune hyperparameters (e.g., alpha for Lasso).

6. Model Evaluation
Make predictions on the test set.
Evaluate the models using Mean Squared Error (MSE) and R-squared (R²) score.
Compare the performance of different models.

7. Visualization
Plot actual vs. predicted values to visualize the model's performance.
Visualize feature importance (for Lasso regression) to understand which features are most
