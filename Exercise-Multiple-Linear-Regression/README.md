# Multiple Linear Regression Exercise

This project demonstrates the implementation of **Multiple Linear Regression** using Python and Scikit-Learn.  
The objective is to understand how multiple independent variables influence a target variable and how regression models can be used for prediction.

The exercise uses a synthetic dataset to analyze how **project size and deadline constraints affect the pricing of a website development project**.

---

# Problem Statement

Freelancers and software developers often need to estimate the cost of a project based on the scope and timeline.

The goal of this exercise is to predict the **recommended project rate (INR)** using the following features:

- Number of pages in the website
- Project deadline in days

By analyzing historical project data, a regression model can estimate a fair project price.

---

# Dataset Description

The dataset consists of **30 project records** containing:

| Feature | Description |
|------|------|
| pages | Number of pages required for the website |
| deadline_days | Project completion deadline |
| rate_inr | Project cost in Indian Rupees |

The dataset is synthetic and created for educational purposes.

According to the dataset statistics shown in the analysis:

- Average pages ≈ **8.83**
- Average deadline ≈ **10.93 days**
- Average project rate ≈ **₹16,833**.

---

# Data Visualization

Scatter plots were used to visualize the relationship between features and price:

1. **Pages vs Rate**
2. **Deadline vs Rate**

The plots show that:

- Project cost increases with the number of pages
- Shorter deadlines tend to increase project pricing due to urgency. 

---

# Model Implementation

The following steps were used to build the model:

1. Import required libraries
2. Create dataset
3. Perform exploratory analysis
4. Visualize relationships
5. Prepare training data
6. Split dataset into training and testing sets
7. Train the Multiple Linear Regression model
8. Evaluate predictions

The model was implemented using:
LinearRegression() from Scikit-Learn

---

# Model Parameters

The trained model produced the following coefficients:

| Feature | Coefficient |
|------|------|
| Pages | 1786 |
| Deadline Days | -207 |
| Intercept | 3117 |

Interpretation:

- Each additional page increases the project rate by approximately **₹1786**.
- Each additional day in the deadline slightly reduces urgency, lowering the price by about **₹207**.

---

# Model Performance

Model accuracy was evaluated using **R² Score**.
R² Score ≈ 0.963


This indicates that the model explains about **96% of the variance in project pricing**. 

---

# Example Prediction

Question:

What should be the recommended rate for a project with:

- **10 pages**
- **5-day deadline**

Predicted recommended price:
₹19,942


This demonstrates how the model can assist freelancers in pricing projects based on scope and urgency. 

---

# Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-Learn
- Jupyter Notebook

---

# Learning Outcomes

Through this exercise, the following concepts were practiced:

- Multiple Linear Regression
- Feature relationship analysis
- Data visualization
- Model training and evaluation
- Predictive analytics

---

# Files Included

Exercise-Multiple-Linear-Regression
│
├── Exercise - Multiple Linear Regression.ipynb  
├── Exercise - Multiple Linear Regression.pdf  
└── README.md

---

# Conclusion

This exercise demonstrates how multiple variables can influence a prediction outcome in regression models.  
By incorporating multiple features such as project size and deadline constraints, the model provides more realistic pricing predictions compared to simple linear regression.

