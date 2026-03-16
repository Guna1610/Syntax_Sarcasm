# Regularization in Linear Models Using Real-World Data

This project explores how **regularization techniques improve the performance of linear regression models** by controlling overfitting.

The study compares three popular regularization methods:

* Ridge Regression (L2 Regularization)
* Lasso Regression (L1 Regularization)
* Elastic Net Regression (Combination of L1 and L2)

The analysis is performed using the **California Housing Dataset** to understand how regularization affects training error, testing error, and model coefficients.

---

# Project Objective

The objectives of this project are to:

* Understand the limitations of ordinary linear regression
* Learn how regularization improves generalization
* Compare Ridge, Lasso, and Elastic Net models
* Study coefficient shrinkage behavior
* Analyze training vs testing error trends
* Understand feature selection in Lasso regression

---

# Dataset Description

The project uses the **California Housing Dataset**, which contains information about housing districts in California.

Features include variables such as:

* Median income
* Average number of rooms
* Population
* Housing age
* Location attributes

The target variable represents **median house value**.

The dataset was obtained using:

```
from sklearn.datasets import fetch_california_housing
```

Before training the models, features were standardized using **StandardScaler** to ensure proper regularization behavior.

---

# Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Scikit-Learn
* Jupyter Notebook

---

# Models Implemented

The following models were implemented and compared.

## Linear Regression

Baseline model without regularization.

This model minimizes **Mean Squared Error (MSE)** but may overfit when features have high variance.

---

## Ridge Regression (L2 Regularization)

Ridge adds a penalty proportional to the **square of the coefficients**.

Loss Function:

MSE + λ Σ (w²)

Effects:

* Coefficients shrink gradually
* No coefficient becomes exactly zero
* All features remain in the model

---

## Lasso Regression (L1 Regularization)

Lasso adds a penalty proportional to the **absolute value of coefficients**.

Loss Function:

MSE + λ Σ |w|

Effects:

* Some coefficients shrink to exactly zero
* Performs automatic feature selection
* Removes less important features

---

## Elastic Net Regression

Elastic Net combines both L1 and L2 penalties.

Loss Function:

MSE + λ₁ Σ|w| + λ₂ Σ(w²)

Effects:

* Some coefficients shrink smoothly
* Some become zero
* Behavior lies between Ridge and Lasso

---

# Training vs Testing Error Analysis

Training and testing errors were calculated for different **alpha values**.

### Ridge Regression

Observations:

* Training error remains almost constant
* Testing error slightly decreases as alpha increases
* No sudden spike in error

This shows Ridge controls coefficient magnitude without removing features.

---

### Lasso Regression

Observations:

* Training and testing errors increase sharply when alpha becomes large
* Excessive regularization removes useful features

This demonstrates how too much regularization can cause **underfitting**.

---

### Elastic Net Regression

Observations:

* Error behavior lies between Ridge and Lasso
* Error increases more gradually compared to Lasso

Elastic Net balances feature elimination and coefficient shrinkage.

---

# Coefficient Shrinkage Analysis

Coefficient shrinkage plots illustrate how model parameters change as regularization strength increases.

### Ridge Regression

* All coefficients shrink gradually
* None become exactly zero

### Lasso Regression

* Several coefficients drop exactly to zero
* Performs automatic feature selection

### Elastic Net

* Some coefficients shrink smoothly
* Some are reduced to zero

---

# Model Comparison

After tuning the regularization parameter α, the models were compared based on **lowest test MSE**.

| Model            | Best Test MSE |
| ---------------- | ------------- |
| Ridge Regression | ~0.529        |
| Lasso Regression | ~0.528        |
| Elastic Net      | ~0.528        |

The **Lasso model achieved the lowest test error**, showing the best generalization performance on this dataset.

---

# Why Regularization Improves Performance

Without regularization, models may assign large weights to features that capture noise instead of meaningful patterns.

Regularization improves performance by:

* Penalizing large coefficients
* Reducing model complexity
* Preventing overfitting
* Improving generalization on unseen data

As the regularization strength increases, test error initially decreases before increasing again, showing the balance between **underfitting and overfitting**.

---

# Key Learning Outcomes

Through this project, the following concepts were explored:

* Linear Regression limitations
* Ridge Regression (L2 regularization)
* Lasso Regression (L1 regularization)
* Elastic Net Regression
* Feature scaling
* Training vs testing error analysis
* Coefficient shrinkage visualization
* Feature selection using Lasso
* Bias-variance tradeoff

---

# Files Included

Regularization-Linear-Models
│
├── Assignment-2.ipynb
├── Assignment-2.pdf
└── README.md

---

# Conclusion

This project demonstrates how regularization improves the performance of linear models by controlling model complexity.

While Ridge reduces coefficient magnitude without removing features, Lasso performs feature selection by eliminating less important variables. Elastic Net combines the strengths of both approaches.

Selecting the appropriate regularization method helps create **stable, interpretable, and generalizable machine learning models**.
