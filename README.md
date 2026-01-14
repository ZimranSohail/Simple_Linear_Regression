# Linear Regression From Scratch (Python)

A Jupyter Notebook–based implementation of **Simple Linear Regression from scratch using NumPy**, focused on building an intuitive understanding of **Ordinary Least Squares (OLS)**. The project manually computes model parameters and evaluation metrics, visualizes results, and validates them against **scikit-learn** using the **ISLP Advertising dataset**.

---

## 📌 Project Overview

This project implements **Ordinary Least Squares (OLS)** linear regression without using machine learning libraries. The goal is to bridge theory and practice by coding the algorithm directly from its mathematical formulation and validating the results using `sklearn.linear_model.LinearRegression`.

The model is trained on the **Advertising dataset**, predicting **Sales** based on **TV advertising budget**.

---

## 🎯 Objectives

* Understand the mathematics behind linear regression
* Implement regression using NumPy only
* Manually compute evaluation metrics
* Visualize model predictions
* Compare results with scikit-learn

---

## 🧠 Concepts Covered

* Mean, variance, and covariance
* Least Squares estimation
* Linear regression assumptions
* Model evaluation metrics:

  * Residual Sum of Squares (RSS)
  * Mean Squared Error (MSE)
  * R² Score
  * Residual Standard Error (RSE)
* Model validation

---

## 📊 Dataset

* **Name:** Advertising Dataset
* **Source:** ISLP
* **Feature Used:** `TV`
* **Target Variable:** `sales`

### Preprocessing Steps

* Removed unnecessary index column
* Checked for missing values
* Ensured numeric data types

---

## ⚙️ Implementation Details

The project defines a custom `Linear_regression` class with the following methods:

* `fit(x, y)` – Estimates slope and intercept using closed-form equations
* `predict(x)` – Predicts output values
* `RSS(x, y)` – Computes Residual Sum of Squares
* `mse(x, y)` – Computes Mean Squared Error
* `R2(x, y)` – Computes coefficient of determination
* `RSE(x, y)` – Computes Residual Standard Error

All computations are implemented **from scratch using NumPy**.

---

## 📈 Results & Visualization

* Scatter plot of TV advertising vs Sales
* Regression line overlaid on actual data
* Printed evaluation metrics for model assessment

The regression line closely matches the scikit-learn implementation.

---

## 🔍 Validation with scikit-learn

The custom implementation is compared with `sklearn.linear_model.LinearRegression` by evaluating:

* Intercept
* Coefficient
* R² Score

The results are nearly identical, confirming the correctness of the implementation.

---

## 🚀 How to Run

This project is implemented as a **Jupyter Notebook**.

1. Clone the repository

````bash
git clone https://github.com/ZimranSohail/linear-regression-from-scratch.git
cd linear-regression-from-scratch
```bash
git clone https://github.com/ZimranSohail/linear-regression-from-scratch.git
cd linear-regression-from-scratch
````

2. Install dependencies

```bash
pip install -r requirements.txt
```

3. Run the script

```bash
jupyter notebook linear_regression_from_scratch.ipynb
```

---

## 🧪 Limitations

* Supports only **simple linear regression**
* No train-test split (educational focus)
* No regularization techniques applied

---

## 🔮 Future Improvements

* Extend to multiple linear regression
* Implement gradient descent
* Add train/test split
* Add residual and diagnostic plots
* Convert into a reusable Python package

---

## 📚 References

* *An Introduction to Statistical Learning*
* scikit-learn documentation

---

## 🙌 Author

**Zimran Sohail**
Aspiring AI Researcher & Data Scientist
Skills: Python, NumPy, Pandas, SQL, Machine Learning Fundamentals

---

⭐ If you found this project useful, consider starring the repository!
