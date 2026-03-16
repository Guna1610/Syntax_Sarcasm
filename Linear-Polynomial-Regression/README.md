# Linear and Polynomial Regression Using Synthetic Data

This project demonstrates the difference between **Linear Regression** and **Polynomial Regression** using synthetic data.

The objective of this exercise is to understand how regression models behave when modeling **non-linear relationships** and how the **polynomial degree affects model performance, bias, and variance**.

The project also explores **training vs testing error**, **overfitting**, and **model complexity**.

---

# Project Objective

The goals of this project are to:

- Understand how linear regression works
- Learn how polynomial regression models non-linear relationships
- Analyze how model complexity affects prediction performance
- Study the **bias-variance tradeoff**
- Observe how training and testing errors behave as model complexity increases

---

# Dataset Description

A **synthetic dataset** was generated using NumPy.

The dataset contains:

- **100 input values (X)** evenly spaced between **-3 and 3**
- Target values **Y generated using a sinusoidal function with noise**
y = sin(x) + noise

Gaussian noise was added to simulate real-world imperfect data. 

This allows us to test how regression models handle **non-linear patterns**.

---

# Technologies Used

- Python
- NumPy
- Matplotlib
- Scikit-Learn
- Jupyter Notebook

---

# Model Implementation

The following steps were performed:

1. Generate synthetic dataset
2. Split dataset into training and testing sets
3. Transform input features using PolynomialFeatures
4. Train Linear Regression on polynomial features
5. Visualize prediction curves
6. Compute training and testing errors
7. Analyze model behavior for different polynomial degrees

Polynomial degrees tested: [1, 3, 5, 9, 12, 15, 18, 20, 23, 27, 29, 30]


Each degree represents a different model complexity.

---

# Linear vs Polynomial Regression

### Linear Regression
Linear regression fits a straight line to the data.

It works well when the relationship between variables is linear.

However, when the data follows a **non-linear pattern**, a straight line cannot capture the underlying structure.

---

### Polynomial Regression

Polynomial regression extends linear regression by transforming the input features into higher-degree polynomial terms.

Example transformation:x → [1, x, x², x³, ...]


This allows the model to fit **curved relationships** in the data.

---

# Bias-Variance Tradeoff

The polynomial degree determines model complexity.

| Polynomial Degree | Bias | Variance | Model Behavior |
|---|---|---|---|
| Low (1–3) | High | Low | Underfitting |
| Medium (5–9) | Balanced | Balanced | Best Fit |
| High (18–30) | Low | High | Overfitting |

Low-degree models cannot capture the true pattern, while very high-degree models memorize the training data. 

---

# Loss Function

Linear regression models are trained by minimizing **Mean Squared Error (MSE)**.

MSE measures the average squared difference between predicted and actual values.
MSE = (1/n) Σ (y_true - y_pred)^2


Squaring the errors ensures:

- Positive and negative errors do not cancel out
- Larger errors are penalized more heavily
- Optimization becomes smoother and easier.

---

# Training vs Testing Error

Training and testing errors were calculated for different polynomial degrees.

Observations:

### Training Error
Training error decreases as polynomial degree increases.

This happens because complex models can fit the training data very closely.

### Testing Error
Testing error initially decreases but later increases when the model becomes too complex.

This occurs because the model begins fitting noise in the training data.

The graph clearly shows this behavior. 

---

# Overfitting Analysis

Overfitting occurs when a model learns the training data too well, including noise.

From the analysis:

- Overfitting begins around **polynomial degree 18–23**
- Model performance worsens after **degree 27**
- Prediction curves become unstable near boundaries.

---

# Best Polynomial Degree

The optimal polynomial degree lies between:5 and 9


This range produces:

- Smooth prediction curves
- Low test error
- Balanced bias and variance

This represents the best generalization performance. 

---

# Files Included
Linear-Polynomial-Regression
│
├── Assignment -1.ipynb
├── Assignment - 1.pdf
└── README.md


---

# Key Learning Outcomes

Through this project, the following concepts were practiced:

- Linear Regression
- Polynomial Regression
- Feature transformation
- Model complexity
- Bias-Variance tradeoff
- Training vs testing error
- Overfitting and underfitting analysis

---

# Conclusion

This project highlights how model complexity affects regression performance.

While simple models fail to capture complex relationships, overly complex models can overfit the data.

Choosing the correct polynomial degree ensures the best balance between **bias and variance**, resulting in accurate and generalizable predictions.

