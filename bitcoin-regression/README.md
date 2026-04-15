# 🪙 Bitcoin Price Prediction Using Machine Learning

## 📌 Project Overview
This project focuses on predicting the **closing price of Bitcoin** using machine learning regression algorithms. By leveraging historical market data, the model learns relationships between key price indicators and the closing price.

The goal is to evaluate and compare the performance of different regression models in predicting Bitcoin prices.

---

## 📊 Dataset Description
The dataset contains **7,510,729 records** of historical Bitcoin price data.

### Features:
- Timestamp
- Open
- High
- Low
- Close (Target Variable)
- Volume

### Data Quality:
- No missing values
- No duplicate records
- All features are numerical

---

##  Data Preprocessing
The following preprocessing steps were performed:

- Converted **Timestamp** from Unix format to datetime
- Sorted dataset chronologically based on time
- Verified data consistency (no nulls or duplicates)

---

##  Feature Selection

### Input Features (X):
- Open
- High
- Low
- Volume

### Target Variable (y):
- Close price

---

##  Train-Test Split
The dataset was split into:
- **70% Training Data**
- **30% Testing Data**

This ensures proper evaluation on unseen data.

---

##  Feature Scaling
Feature scaling was applied using standardization to normalize input variables. This step is particularly important for distance-based models like KNN.

---

## Models Implemented

###  Linear Regression
A statistical method that models the relationship between input features and the target variable using a linear equation.

###  K-Nearest Neighbors (KNN) Regression
A non-parametric model that predicts values based on the average of the nearest data points using distance metrics.

---

## Evaluation Metrics
The models were evaluated using:

- **MAE (Mean Absolute Error):** Measures average prediction error  
- **MSE (Mean Squared Error):** Penalizes larger errors  
- **R² Score:** Measures how well the model explains variance  

---

##  Results

| Model               | MAE   | MSE     | R² Score        |
|--------------------|------|---------|-----------------|
| Linear Regression  | 4.40 | 134.91  | 0.99999986      |
| KNN Regression     | 8.52 | 1546.41 | 0.99999839      |

---

##  Model Comparison
- **Linear Regression** achieved lower error values and better overall performance  
- **KNN Regression** performed well but showed higher prediction errors  

---

## 📌 Conclusion
Both models performed exceptionally well, indicating a strong relationship between the selected features and Bitcoin closing price. However, **Linear Regression** proved to be more suitable due to its simplicity and superior accuracy.

---

## 🛠️ Tools & Libraries
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib / Seaborn

---

## Project Structure
