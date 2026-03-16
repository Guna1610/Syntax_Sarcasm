# Linear Regression Exercise

This project demonstrates the implementation of **Simple Linear Regression** using Python and Scikit-Learn.  
The goal of this exercise is to understand how a single independent variable can be used to predict a target variable using a regression model.

The project analyzes the relationship between **early engagement on a video (likes in the first hour)** and the **total number of views the video eventually receives**.

---

# Problem Statement

Content creators often want to estimate how well a video will perform shortly after it is uploaded.

The goal of this exercise is to determine whether the number of **likes received during the first hour** can help predict the **total number of views** a video will achieve.

If a strong relationship exists, this information can help creators:

- Evaluate video performance early
- Adjust promotion strategies
- Predict audience reach

---

# Dataset Description

The dataset used in this exercise is a **synthetic dataset created for learning purposes**.

It contains the following variables:

| Feature | Description |
|------|------|
| first_hour_likes | Number of likes received within the first hour of upload |
| total_views | Total number of views the video receives |

Each row represents a video and its performance metrics.

---

# Data Visualization

A scatter plot was used to visualize the relationship between:

**First Hour Likes vs Total Views**

The visualization helps observe whether a **linear relationship exists between early engagement and total reach**.

If the data points follow a roughly straight pattern, a linear regression model can effectively capture the relationship.

---

# Model Implementation

The following steps were followed to build the model:

1. Import required libraries
2. Create the dataset
3. Perform exploratory data analysis
4. Visualize the relationship between variables
5. Prepare feature and target variables
6. Split the dataset into training and testing sets
7. Train a Linear Regression model
8. Evaluate the predictions

The model was implemented using:
LinearRegression() from Scikit-Learn


---

# Model Interpretation

The regression model calculates two key parameters:

**Slope (Coefficient)**  
Represents how much the total views increase when first-hour likes increase by one unit.

**Intercept**  
Represents the predicted number of views when the number of first-hour likes is zero.

These parameters define the regression equation:
Total Views = (Slope × First Hour Likes) + Intercept


---

# Model Evaluation

Predictions were generated using the trained model on the test dataset.

The predicted values were compared with actual values to observe how well the model performs.

This step helps determine whether the model can accurately estimate video performance.

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

- Simple Linear Regression
- Feature and target variable selection
- Data visualization using scatter plots
- Train-test data splitting
- Model training using Scikit-Learn
- Generating predictions using regression models

---

# Files Included
Exercises-Linear-Regression
│
├── Assignment-1 Linear Regression.ipynb
└── README.md


---

# Conclusion

This exercise demonstrates how **early engagement metrics can be used to predict the future performance of content**.

Simple Linear Regression provides a straightforward method for modeling relationships between two variables and forms the foundation for more advanced machine learning models.
