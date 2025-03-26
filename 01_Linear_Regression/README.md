# Salary Prediction Using Linear Regression

## Overview
This project demonstrates a simple implementation of a **Linear Regression** model using Python and scikit-learn to predict average salary estimates based on job-related features. The exercise is built on a cleaned dataset of job listings containing various attributes like company rating, job state, years since founding, and required technical skills such as Python, Excel, etc.

## Objective
The main goal of this exercise is to:

1. Explore the relationship between job features and salary expectations.  
2. Apply linear regression to build a predictive model for average salaries.  
3. Evaluate the performance of the model using metrics such as **Mean Squared Error (MSE)**.

## Dataset
The dataset used is `salary_data_cleaned.csv`, which includes 28 columns:

- Job Title, Salary Estimate, Rating, Company Name, Location, etc.  
- `avg_salary` is used as the **target variable** for prediction.

## Tools and Libraries
- `pandas` for data manipulation  
- `scikit-learn` for model building and evaluation

## Model Training Steps
1. Imported the dataset and selected only numerical columns.  
2. Split the data into a 70:30 train-test ratio.  
3. Trained a `LinearRegression` model to predict `avg_salary`.  
4. Evaluated the model using **Mean Squared Error**, which turned out to be very close to 0, indicating high accuracy on the test set.

## Key Learning Outcomes
- Understood how to preprocess and select numeric features for regression models.  
- Learned how to train and evaluate a **Linear Regression** model.  
- Observed how even simple linear models can provide strong predictive power in structured datasets.
