# 🛍️ Ecommerce Predictive Modeling

This project focuses on building and evaluating multiple regression models to **predict yearly customer spending** based on their behavior and engagement metrics in an e-commerce platform.  
The goal is to explore different modeling techniques, perform feature selection, and identify the best-performing model for accurate predictions.

---

## 📝 Project Overview

The goal is to understand customer purchasing patterns and build predictive models using three regression approaches:

- 🤖 **Linear Regression**  
- 🖥️ **Support Vector Regression (SVR)**  
- 🧠 **Multilayer Perceptron (MLP)**

Each model is evaluated using **R², MAE, and RMSE**, and feature selection is applied to optimize performance.

---

## 📁 Project Structure

```
Ecommerce-Predictive-Modeling/
│
├── 📂 notebooks/                            # Main notebooks (EDA & data preprocessing, data modeling)
├── 📂 plots/                                # Visualizations from the notebooks 
├── 📄 requirements.txt                      # Project dependencies
├── 📄 README.md                             # Project documentation
└── 📂 data/                                 # Dataset folder 
```

---

## 📂 Dataset

The dataset contains customer information with the following features:

- Avg. Session Length  
- Time on App  
- Time on Website  
- Length of Membership  
- Yearly Amount Spent (**Target**)  

> The dataset used in this project is included in the repository as '[📊 Dataset](data/Clients_Ecommerce.csv)'.

---

## 🔑 Key Features

- 📈 **Exploratory Data Analysis (EDA):** Pairplots, correlation heatmaps, and distribution charts to explore patterns.  
- ⚙️ **Data Preprocessing:** Dealing with missing values, duplicates, and feature scaling.  
- 🛠️ **Modeling & Evaluation:** Default models, cross-validation, GridSearch, and feature selection for optimal results.  
- 💡 **Insights & Benchmarking:** Comparison of models’ performance and identification of the best model.  

---

## 🧰 Models & Techniques

- **Linear Regression** (Default, Cross-validation, Feature Selection, Grid Search)  
- **Support Vector Regression (SVR)** (Default, Cross-validation, Feature Selection, Grid Search)  
- **Multilayer Perceptron (MLP)** (Default, Cross-validation, Feature Selection, Grid Search)  
- **Feature Selection** using `mutual_info_regression` and percentile-based selection  
- **Evaluation Metrics:** R², MAE, RMSE

---

## 📊 Benchmark Summary

| Model | R² Score | MAE | RMSE |
|-------|----------|-----|------|
| 🧠 MLP (GridSearch + CV) | 0.985 | 0.098 | 0.016 |
| 🖥️ SVR (GridSearch + Feature Selection) | 0.984 | 0.093 | 0.014 |
| 🤖 Linear Regression (Feature Selection) | 0.986 ✅ | 0.090 ✅ | 0.013 ✅ |

**Top 3 features:** `Avg. Session Length`, `Time on App`, `Length of Membership`.

---

## 💡 Insights

- Feature selection significantly improves model performance. ✨  
- All models achieve **high R² scores (>0.98)**, showing strong predictive accuracy.  
- **Linear Regression** provides the best combination of interpretability, accuracy and simplicity for deployment.  
- **MLP and SVR** capture non-linear patterns effectively, offering competitive results.  

---

## 🛠️ Tech Stack

- Python 🐍  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn
- scikeras

---

## 🚀 Usage

1. Clone this repository:
   ```bash
   git clone https://github.com/HajarLHA/Ecommerce-Predictive-Modeling.git
   cd Ecommerce-Predictive-Modeling
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## 📝 Future Improvements

- 🔸 Experiment with **ensemble models** (e.g., Random Forest, Gradient Boosting).  
- 🔸 Deploy the best model as a simple API using FastAPI or Flask.  
- 🔸 Add automated visualizations and dashboards.

---

👩‍💻 Created by *Hajar Lhamyani* – Data Scientist & Analyst | Machine Learning Engineer
