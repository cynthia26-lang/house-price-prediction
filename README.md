# house-price-prediction
Predicting house prices in King County using Python, EDA, and Machine Learning (Linear Regression &amp; Random Forest)

# House Price Prediction using Python & Machine Learning

## Overview  
This project predicts **house prices in King County, USA (2014–2015)** using data analysis and machine learning.  
The dataset contains **21,613 records and 21 features**, including house size, location, condition, and year built.

The main goal is to understand which factors drive house prices and to build a predictive model.

---

## Objectives  
- Perform **Exploratory Data Analysis (EDA)** to identify key factors affecting prices.  
- Engineer new features such as **house_age** , **renovated** and **price_per_sqft**.  
- Build and evaluate ML models: **Linear Regression** and **Random Forest**.  
- Compare performance using **R² score** and **RMSE**.  

---

## Dataset  
- **Source:** [Kaggle – House Sales in King County, USA](https://www.kaggle.com/datasets/harlfoxem/housesalesprediction)  
- **Rows:** 21,613  
- **Columns:** 21  

Key Features:  
- `sqft_living`: Living area size  
- `bedrooms`, `bathrooms`  
- `floors`, `waterfront`, `view`, `condition`, `grade`  
- `yr_built`, `yr_renovated`  
- `lat`, `long`, `zipcode`  

---

## Models & Performance  

| Model              | R² Score | RMSE (USD) |
|--------------------|----------|------------|
| Linear Regression  | ~0.68    | ~202,000   |
| Random Forest      | ~0.87    | ~128,000   |

**Random Forest performed better** than Linear Regression.  
Most important features: **sqft_living, grade, lat, long**.  

---

## Feature Importance  
Random Forest identified the following as most important:  
- **sqft_living** (house size)  
- **grade** (overall quality)  
- **latitude & longitude** (location)  
- **renovated**  

---

## Conclusion  
- Location and house size are the strongest predictors of price.  
- Random Forest outperformed Linear Regression with R² ≈ 0.87.  
- Future improvements:  
  - Apply **log-transform** to prices  
  - Hyperparameter tuning  
  - Try **XGBoost/LightGBM** for boosting accuracy to 80%+  

---

