# Calories Burnt Prediction using Machine Learning

This project aims to build a machine learning model that predicts the number of calories burnt by an individual during physical activity based on several biological and workout-related parameters.

## Dataset

The data is sourced from [Kaggle](https://www.kaggle.com/). It includes two CSV files:
- `calories.csv`
- `exercise.csv`

These were merged on `User_ID` to create a final dataset with the following features:
- Age
- Gender
- Height
- Weight
- Duration
- Heart Rate
- Body Temperature
- Calories (Target Variable)

## Objective

To predict the `Calories` column using machine learning regression techniques.

---

## Tools & Libraries Used

- Python
- NumPy
- Pandas
- Seaborn & Matplotlib (EDA & Visualization)
- Scikit-learn (Preprocessing & Modeling)
- XGBoost
- RandomForest

---

## Exploratory Data Analysis (EDA)

- Explored feature distributions and correlations
- Identified and removed data leakage from features like `Weight` and `Duration`
- Visualized the relationship between variables and target (`Calories`)
- Categorical encoding: Converted `Gender` into numerical format

---

## Model Training

Used the following regression models:

- Linear Regression
- Ridge Regression
- Lasso Regression
- XGBoost Regressor
- Random Forest Regressor

### Evaluation Metric:
- **Mean Absolute Error (MAE)** was used to evaluate model performance

---

## Best Performing Models

| Model                  | Validation MAE |
|------------------------|----------------|
| Random Forest Regressor| ~10.45         |
| XGBoost Regressor      | ~10.12         |
| Linear/Ridge/Lasso     | ~18            |

Random Forest and XGBoost outperformed the others in terms of lower validation error.

---

## Key Takeaways

- Identified and resolved potential **data leakage**
- Applied **feature normalization** using `StandardScaler`
- Compared model performance using MAE
- Showcased the real-world application of regression models in health and fitness



