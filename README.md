# Student Performance Prediction using Machine Learning

## Project Overview

This project focuses on predicting students' academic performance using Regression. The notebook demonstrates an end-to-end regression workflow, including data exploration, preprocessing, model development, performance evaluation, and comparison between Linear Regression and Polynomial Regression.

The objective is to identify how study habits and academic-related factors influence student performance and to build an accurate predictive model.

---

## Problem Statement

Educational institutions can benefit from predicting student performance to identify students who may require additional academic support and to better understand the factors affecting learning outcomes.

This project aims to develop regression models capable of predicting a student's **Performance Index** based on several academic and lifestyle features.

---

## Dataset Information

### Dataset Summary

- **Dataset Size:** 10,000 observations × 6 columns
- **Machine Learning Problem:** Supervised Regression
- **Target Variable:** Performance Index

### Features

| Feature | Description |
|----------|-------------|
| Hours Studied | Number of hours studied |
| Previous Scores | Previous examination scores |
| Extracurricular Activities | Participation in extracurricular activities |
| Sleep Hours | Average daily sleep duration |
| Sample Question Papers Practiced | Number of practice papers solved |
| Performance Index | Student performance score (Target Variable) |

### Dataset Quality

- No missing values were found.
- Duplicate records were identified during data inspection.
- Both numerical and categorical variables are present.
- The categorical feature was encoded before model training.

---

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

---

## Project Workflow

Import Dataset

↓

Data Inspection

↓

Exploratory Data Analysis (EDA)

↓

Data Preprocessing

↓

Feature Encoding

↓

Train-Test Split

↓

Linear Regression

↓

Polynomial Regression

↓

Model Evaluation

↓

Model Comparison

↓

Best Model Selection

---

## Exploratory Data Analysis

The notebook includes:

- Dataset structure inspection
- Statistical summary
- Missing value analysis
- Duplicate value analysis
- Feature distribution analysis
- Correlation analysis
- Relationship between input features and target variable

The exploratory analysis helps understand the characteristics of the dataset before model development.

---

## Machine Learning Models

### Linear Regression

A baseline regression model used to establish the relationship between the independent variables and the Performance Index.

Evaluation Metrics:
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

---

### Polynomial Regression

Polynomial features were generated to evaluate whether introducing nonlinear relationships could improve prediction performance over the baseline Linear Regression model.

The performance of the Polynomial Regression model was compared directly with Linear Regression using identical evaluation metrics.

---

## Model Evaluation

The following regression metrics were used:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

These metrics evaluate prediction accuracy and the model's ability to explain variance in the target variable.

---

## Results

| Model | MAE | MSE | RMSE | R² Score |
|-------|------:|------:|------:|------:|
| Linear Regression | 1.6230 | 4.2405 | 2.0592 | 0.9886 |
| Polynomial Regression | 1.6245 | 4.2474 | 2.0609 | 0.9885 |

---

## Best Model

Based on the evaluation metrics, **Linear Regression** performed slightly better than Polynomial Regression.

The results indicate that the relationship between the predictor variables and the target variable is already well captured by a linear model. Introducing polynomial features did not provide a meaningful improvement in predictive performance while increasing model complexity.

---

## Key Learning Outcomes

- End-to-end supervised machine learning workflow
- Exploratory Data Analysis (EDA)
- Data preprocessing techniques
- Feature encoding
- Correlation analysis
- Train-test splitting
- Linear Regression
- Polynomial Regression
- Model evaluation using regression metrics
- Comparative model analysis
- Interpretation of regression performance metrics

---

## Future Improvements

- Evaluate additional regression algorithms such as Ridge, Lasso, Elastic Net, Decision Tree Regressor, Random Forest Regressor, and Gradient Boosting Regressor.
- Perform feature engineering to explore interaction effects between variables.
- Apply cross-validation for more robust model evaluation.
- Investigate feature importance using ensemble-based regression models.
- Deploy the best-performing model as a web application using Flask or Streamlit.

---

## Conclusion

This project demonstrates a complete regression-based machine learning pipeline for predicting student performance. The dataset was explored, preprocessed, and used to train both Linear Regression and Polynomial Regression models. Model performance was evaluated using standard regression metrics, and the results showed that Linear Regression achieved slightly better predictive performance than Polynomial Regression. The high R² score indicates that the selected features explain a substantial proportion of the variation in student performance. Overall, the project highlights the importance of systematic data preprocessing, appropriate model selection, and quantitative evaluation when developing predictive machine learning solutions.
