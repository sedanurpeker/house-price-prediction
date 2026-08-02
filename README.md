# 🏠 House Price Prediction

[![Python](https://img.shields.io/badge/Python-3.9%2B-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-F7931E?logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![XGBoost](https://img.shields.io/badge/XGBoost-Gradient_Boosting-red)](https://xgboost.readthedocs.io/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

This project uses the Kaggle **"House Prices - Advanced Regression Techniques"** dataset to build machine learning models that predict a house's sale price based on its various features.

## 📑 Table of Contents

- [Dataset](#-dataset)
- [Project Features](#-project-features)
- [Tech Stack](#-tech-stack)
- [Getting Started](#-getting-started)
- [Model Comparison](#-model-comparison)
- [Project Structure](#-project-structure)
- [Author](#-author)

## 📊 Dataset

- **Source:** [House Prices - Advanced Regression Techniques (Kaggle)](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)
- **Description:** The dataset contains 80+ variables describing the physical and locational characteristics of residential homes.
- **Target variable:** `SalePrice` — the home's sale price.
- **File:** `train.csv`

## ✨ Project Features

- **Data Cleaning:** Missing values filled using median or `'None'`
- **Data Visualization:** Distribution and correlation analysis with Seaborn
- **Modeling:**
  - Linear Regression
  - Random Forest Regressor
  - XGBoost Regressor
- **Model Evaluation:** RMSE (Root Mean Squared Error) and MAPE (Mean Absolute Percentage Error)
- **Feature Importance Analysis:** Feature importance plot via Random Forest

## 🛠 Tech Stack

- Python 3.9+
- Pandas / NumPy
- Matplotlib / Seaborn
- Scikit-Learn
- XGBoost

## 🚀 Getting Started

1. Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost
```

2. Run the project:

```bash
python main.py
```

## 📈 Model Comparison

| Model | Mean RMSE | RMSE Std. Dev. | MAPE (%) |
|---|---|---|---|
| Linear Regression | 0.155164 | 0.029752 | 10.079832 |
| Random Forest | 0.143166 | 0.008549 | 10.174023 |
| **XGBoost** | **0.134444** | 0.012261 | **9.619548** |

XGBoost achieved the lowest error overall, with the best RMSE and MAPE among the three models.

## 📂 Project Structure

```
house-price-prediction/
├── main.py       → Modeling and analysis code
├── train.csv     → Kaggle dataset
└── README.md
```

## 👤 Author

**Sedanur Peker**
