# Tech Salaries Analysis

Multiple regression and regularized regression analysis of self-reported 2017 US tech industry salaries. This project explores key predictors of total annual compensation and investigates potential gender pay disparities using logistic regression models.

---

## Project Overview

This project analyzes a dataset of over 62,000 tech industry workers in the US from 2017. It uses linear regression, ridge regression, lasso regression, and logistic regression to identify important predictors of total compensation, evaluate model improvements from regularization, and assess gender pay gap controversies.

The analysis covers:
- Identification of the best predictor of total compensation via multiple linear regression  
- Comparison of ordinary least squares (OLS) to ridge and lasso regression models  
- Examination of the influence of compensation on gender via logistic regression  
- Predictive modeling of high vs low pay based on demographic and performance variables  

---

## Dataset

The dataset `techSalaries2017.csv` includes the following key columns (among others):

1. Company  
2. Job title  
3. Office location  
4. Total annual compensation ($) — Outcome variable  
5. Base salary ($)  
6. Stock grants ($)  
7. Bonus payments ($)  
8. Years of relevant experience  
9. Time with company  
10. Gender  
11–15. Terminal degree indicators (Masters, Bachelors, Doctorate, High School, Some College)  
16–20. Self-identified race/ethnicity indicators  
21–22. Race and education as qualitative variables  
23. Age  
24. Height (inches)  
25. Zodiac sign  
26. SAT score  
27. GPA  

Note: Some data fields have missing values (NA), especially education and race variables, requiring careful preprocessing.

---

## Methods

- Data cleaning and preprocessing to handle missing values and encode categorical variables  
- Multiple linear regression to identify the strongest predictors of total compensation  
- Ridge regression to control for multicollinearity and prevent overfitting; selection of optimal lambda via cross-validation  
- Lasso regression for feature selection and sparsity analysis; optimal lambda selection  
- Logistic regression models predicting gender from compensation with and without covariates  
- Logistic regression predicting high vs low pay from demographic and performance variables  
- Visualization of regression coefficients, error metrics, and model comparisons

---

## Results Summary

- The best predictor of total compensation identified via multiple linear regression was [Insert Predictor], explaining X% of variance (R² = 0.XX).  
- Ridge regression improved the model by reducing overfitting, with an optimal lambda of [Insert λ value].  
- Lasso regression shrunk [Insert Number] coefficients to zero, highlighting key predictors while simplifying the model, with an optimal lambda of [Insert λ value].  
- Logistic regression revealed a significant association between compensation and gender, even when controlling for other factors, suggesting [brief interpretation].  
- Predictive modeling of high vs low pay achieved [Insert accuracy or relevant metric] using variables including years of experience, age, height, SAT score, and GPA.  
- Distributions of salary, height, and age showed [describe normality or skewness], which [does/does not] align with expectations given the dataset context.  
- Additional insights: [Optional interesting fact or finding].

*Include plots of regression coefficients, residuals, lambda tuning curves, and classification metrics.*

---

## How to Run

1. Clone the repository:  
   ```bash
   git clone <repo-url>
