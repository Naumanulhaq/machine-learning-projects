# Titanic Survival Prediction Using Logistic Regression

## Overview  
This project demonstrates the use of **Logistic Regression** to predict passenger survival from the Titanic dataset. Using Python and scikit-learn, the model learns patterns from the dataset to predict which passengers were more likely to survive based on factors like **sex**, **class**, **age**, **parch**, and **sibsp**. The exercise focuses on binary classification and highlights the importance of proper data preprocessing.

---

## Objective  

- Predict survival using logistic regression.  
- Understand how categorical and numerical features influence prediction.  
- Observe how converting string values (like `Sex`) to binary affects model performance.  

---

## Dataset  

The dataset contains the following features:

- `Pclass` – Passenger Class (1 = 1st, 2 = 2nd, 3 = 3rd)  
- `Sex` – Gender (converted to binary: female = 0, male = 1)  
- `Age` – Age of passenger
- `SibSp` – Number of siblings/spouses aboard  
- `Parch` – Number of parents/children aboard 
- `Survived` – Target variable (1 = Survived, 0 = Did not survive)

---

## Tools and Libraries  

- `scikit-learn` for machine learning  

---

## Data Preprocessing  

**Handling Categorical Variables**  
- Converted `sex` from string to binary (`male = 1`, `female = 0`).  
- This step was crucial in improving model performance.

**Missing Values**  
- Rows with missing values (especially in `age`) were removed using `dropna()`.

**Feature Selection**  
- Selected relevant columns: `sex`, `pclass`, `age`, `sibsp`, `parch` and `survived`.

---

## Model Training  

- Split the dataset into 70:30 ratio for training and testing sets accordingly.  
- Trained a **Logistic Regression** model using scikit-learn.
- Evaluated using accuracy score and classification metrics.

---

## Results & Accuracy  

The model achieved an accuracy of approximately **83%** on the dataset.

| Preprocessing Step       | Effect on Accuracy     |
|--------------------------|------------------------|
| Without encoding `sex`   | Lower accuracy         |
| With binary `sex` encoding | Accuracy improved |

**Insight**:  
The model learned that **female passengers** had a higher survival rate, improving accuracy when the `Sex` column was properly encoded. This mirrors historical data where women were prioritized during evacuation.

---

## Key Learnings  

- Logistic Regression is effective for binary classification problems.  
- Converting categorical variables like `Sex` to numerical form is essential.  
- Even basic feature engineering can greatly impact model performance.  

---


1. Clone this repo  
2. Install dependencies:

```bash
pip install pandas scikit-learn matplotlib
