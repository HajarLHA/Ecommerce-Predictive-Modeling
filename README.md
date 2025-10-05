# E-commerce Predictive Modeling

This repository contains a portfolio project analyzing **e-commerce customer data** to predict **Yearly Amount Spent** using machine learning models. The project demonstrates skills in **EDA, data preprocessing, feature engineering, modeling, and model evaluation**.

## Project Overview

The goal of this project is to understand customer purchasing patterns and build predictive models using three regression approaches:

- **Linear Regression**  
- **Support Vector Regression (SVR)**  
- **Multilayer Perceptron (MLP)**

Each model is evaluated using **R², MAE, and RMSE**, and feature selection is applied to optimize performance.

## Dataset

The dataset includes customer information with the following features:

- Avg. Session Length  
- Time on App  
- Time on Website  
- Length of Membership  
- Yearly Amount Spent (Target)

> Note: The dataset used in this project is included in the repository as `ecommerce_data.csv`.

## Key Features

- **Exploratory Data Analysis (EDA):** Pairplots, correlation heatmaps, and distribution charts to understand data patterns.  
- **Data Preprocessing:** Scaling, train/test split, and feature selection.  
- **Modeling & Evaluation:** Default models, cross-validation, GridSearch, and feature selection for optimal results.  
- **Insights & Benchmarking:** Comparison of models’ performance and identification of the best model.  

## Benchmark Summary

| Model | R² Score | MAE | RMSE |
|-------|----------|-----|------|
| MLP (GridSearch + CV) | 0.985 | 0.098 | 0.016 |
| SVR (GridSearch + Feature Selection) | 0.984 | 0.093 | 0.014 |
| Linear Regression (Feature Selection) | 0.986 ✅ | 0.090 | 0.013 ✅ |

**Top 3 features** (`Avg. Session Length`, `Time on App`, `Length of Membership`) were used for the best performance across all models.

## Insights

- Feature selection significantly improves model performance.  
- All models achieve high R² scores (>0.98), showing strong predictive capability.  
- Linear Regression provides the **best combination of accuracy and simplicity** for deployment.  
- MLP and SVR effectively capture non-linear patterns, offering competitive performance.  

## Tech Stack

- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/HajarLHA/Ecommerce-Predictive-Modeling.git
