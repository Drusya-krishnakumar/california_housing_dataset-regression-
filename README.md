# 🏠 California Housing Price Prediction – Regression Models

## 🎯 Objective
This project aims to evaluate and compare various regression algorithms on the **California Housing dataset** using supervised learning techniques. The goal is to predict the median house value in California districts based on multiple features.

---

## 📚 Dataset Overview

- **Dataset:** California Housing Dataset (`sklearn.datasets.fetch_california_housing`)
- **Instances:** 20,640
- **Features:** 8 (e.g., median income, house age, population)
- **Target:** Median house value (in $100,000 units)

---

## ⚙️ Preprocessing Steps

- Loaded the dataset using `fetch_california_housing()`
- Converted it into a Pandas DataFrame
- Checked for and confirmed **no missing values**
- Applied **StandardScaler** for feature scaling (essential for SVR)
- Split the data into **80% training** and **20% testing** using `train_test_split()`

---

## 🧠 Models Implemented

| Model No. | Model                      |
|-----------|----------------------------|
| 0         | Linear Regression          |
| 1         | Decision Tree Regressor    |
| 2         | Random Forest Regressor    |
| 3         | Gradient Boosting Regressor|
| 4         | Support Vector Regressor   |

---

## 📊 Performance Comparison

| Model No. | Model                      | MSE       | MAE       | R² Score |
|-----------|----------------------------|-----------|-----------|----------|
| **2**     | **Random Forest**           | **0.1787** | **0.2911** | **0.7956** |
| 3         | Gradient Boosting          | 0.2049    | 0.3227    | 0.7655   |
| 4         | Support Vector Regressor   | 0.2267    | 0.3356    | 0.7407   |
| 0         | Linear Regression          | 0.3165    | 0.4236    | 0.6379   |
| 1         | Decision Tree Regressor    | 0.4148    | 0.4314    | 0.5254   |

---

## 🏁 Conclusion

- ✅ **Best Model:** `Random Forest Regressor` – highest R² and lowest error values.
- ⚠️ **Moderate Models:** `Gradient Boosting`, `SVR` – good performance, especially after scaling.
- ❌ **Weakest Models:** `Linear Regression`, `Decision Tree` – high bias or overfitting.

---

