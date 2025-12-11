# Credit Card Spending Prediction

This project builds a machine learning model to predict a customer’s next-month credit card spending using historical transaction data. It integrates SQL feature engineering, exploratory data analysis, and regression modeling.

## Overview
- Created a SQLite database for customers, transactions, and merchants  
- Generated monthly spending features using SQL (`SUM`, `COUNT`, `AVG`)  
- Performed EDA to understand spending behavior and seasonality  
- Trained multiple regression models to compare performance  
- Identified **Gradient Boosting** as the best predictor of next-month spending  

## Data
- `credit_card_transactions.csv` (was not able to upload directly due to size limits)  
- `BankChurners.csv` (used for SQL demonstration only)

## Machine Learning
**Target variable:** `next_month_spend`  
**Features:** `total_spend`, `num_transactions`, `avg_transaction_amt`, `month`, `quarter`

**Models trained:**
- Linear Regression  
- KNN  
- Decision Tree  
- Random Forest  
- **Gradient Boosting (best performance)**  

**Best Model Results:**
- **RMSE:** ~2125  
- **MAE:** ~1453  
- **R²:** ~0.73  

## How to Run 
1. Open the Jupyter Notebook  
2. Run all cells to create the SQL database, generate features, run EDA, and train the models  

