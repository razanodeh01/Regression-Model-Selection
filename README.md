
# 🚗 Regression Analysis and Model Selection (ML Assignment #2)

## 📄 About the Assignment

A machine learning assignment focused on regression analysis and model selection using a real-world car dataset. It includes data preprocessing, exploratory analysis, linear and non-linear modeling, regularization techniques (LASSO and Ridge), forward feature selection, and hyperparameter tuning using grid search.


## 📦 Dataset Overview

- **Source**: [YallaMotors Cars Dataset on Kaggle](https://www.kaggle.com/datasets/ahmedwaelnasef/cars-dataset/data). 
- **Size**: ~6,750 records, 9 features.  
- **Target Variable**: Car Price (standardized to USD).  
- **Feature Types**:
  - *Categorical*: Country, Brand.  
  - *Numerical*: Engine Capacity, Cylinders, Horsepower, Top Speed, Seats, Price. 


## 🧹 Preprocessing Steps

- Cleaned missing/inconsistent values (e.g., from "Seater" in `top_speed`, "N/A, Electric` in `cylinders`).
- Standardized currencies to USD in the `price` column.
- Used **z-score normalization** for numerical features.
- Encoded categorical features:
  - One-hot encoding for `country`.
  - Label encoding for `brand`.
- Split the dataset into:
  - **60% Training**.
  - **20% Validation**.
  - **20% Test**.


## 📊 Models Implemented

### 🔷 Linear Models
- Built-in Linear Regression (sklearn).
- Linear Regression from scratch (Closed-Form).
- Gradient Descent Linear Regression.
- LASSO (L1 Regularization) with grid search.
- Ridge Regression (L2 Regularization) with grid search.

### 🔶 Non-Linear Models
- Polynomial Regression (degrees 2–6).
- Polynomial + LASSO pipeline with best hyperparameters.


## 🧪 Model Evaluation Metrics

Evaluated using:
- Mean Squared Error (MSE).
- Mean Absolute Error (MAE).
- R-squared (R²).

The final selected model was evaluated on the test set for generalization performance.


## 🧠 Feature Selection

Performed **Forward Feature Selection** to iteratively select the most impactful features based on validation MSE. Identified optimal subsets and visualized improvement metrics across iterations.


## 🔧 Hyperparameter Tuning

Used **Grid Search** to:
- Optimize `alpha` values for LASSO and Ridge.
- Select best polynomial degree for regression (best: degree 4).
- Ensure balance between accuracy and complexity.


## 👥 Authors
- [**Razan Abdalrahman**](https://github.com/razanodeh01)  
- [**Hidaya Mustafa**](https://github.com/HidayaMustafa)

> 📈 *Analyzing car prices with machine learning – one model at a time.*
