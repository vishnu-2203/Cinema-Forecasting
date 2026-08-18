# Movie Audience Prediction using Machine Learning

## Overview

This project focuses on predicting movie theater audience counts using machine learning techniques. The objective is to analyze historical theater data, extract meaningful features, and build predictive models that estimate the expected number of viewers for movie screenings.

The project combines exploratory data analysis, feature engineering, and multiple machine learning models to improve prediction performance. An ensemble approach is used to achieve more reliable results.

## Problem Statement

Predict the number of people attending a movie screening (`audience_count`) based on various factors such as:

- Theater characteristics
- Geographic location
- Time patterns (weekday, monthly trends)
- Historical performance data

Accurate prediction of audience turnout can help theaters optimize scheduling, marketing strategies, and resource allocation.

## Dataset Description

The dataset contains information about movie screenings and theater performance. Key variables include:

- Theater information
- Geographic attributes
- Screening date and time related features
- Historical audience data
- Operational features related to theaters

The target variable used for prediction is:

`audience_count`

## Project Workflow

### 1. Import Libraries
Standard Python libraries for data analysis, visualization, and machine learning were used.

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost

### 2. Data Loading
Training and testing datasets were loaded and inspected to understand the structure and quality of the data.

### 3. Exploratory Data Analysis

EDA was performed to understand patterns and relationships in the data, including:

- Target variable distribution
- Day-of-week patterns
- Monthly trends
- Theater type analysis
- Geographic distribution
- Theater performance rankings
- Weekend vs weekday comparison
- Correlation analysis
- Year-over-year trends
- Data quality checks

These analyses helped identify useful predictive signals in the dataset.

### 4. Feature Engineering

Additional features were created to improve model performance, including:

- Date-based features
- Aggregated statistics
- Encoded categorical variables
- Derived performance indicators

Feature engineering plays a key role in improving prediction accuracy.

### 5. Data Preparation

Before model training:

- Missing values were handled
- Features were scaled where necessary
- Training and validation splits were created

This step ensures the data is suitable for machine learning models.

### 6. Model Training

Multiple models were trained to compare performance.

#### Ridge Regression
A regularized linear model used as a baseline to capture linear relationships.

#### Random Forest
A tree-based ensemble model that captures nonlinear relationships and feature interactions.

#### XGBoost
A gradient boosting algorithm known for high performance in predictive modeling tasks.

### 7. Ensemble Model

Predictions from multiple models were combined using an ensemble approach. This improves prediction stability and reduces model bias.

### 8. Test Data Processing

The same preprocessing and feature engineering steps applied to the training data were also applied to the test dataset to ensure consistency.

### 9. Prediction Generation

Final predictions for `audience_count` were generated using the trained models and ensemble method.

### 10. Submission File Creation

The predictions were formatted into the required submission format.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Jupyter Notebook

## Key Learnings

- Importance of exploratory data analysis in identifying patterns
- Impact of feature engineering on model performance
- Comparison of linear and tree-based machine learning models
- Advantages of ensemble modeling techniques

## Future Improvements

- Hyperparameter tuning using GridSearch or Optuna
- Feature selection techniques
- Advanced ensemble methods such as stacking
- Incorporating additional external data sources
- Deploying the model using a web application or API

## Conclusion

This project demonstrates how machine learning can be used to predict audience turnout for movie screenings. By combining data exploration, feature engineering, and multiple predictive models, the project builds a robust pipeline for estimating audience demand.
