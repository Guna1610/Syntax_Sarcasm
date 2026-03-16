# Coding Practice & Submission

## Overview
This folder contains my hands-on machine learning coding practice projects focused on applying **Linear Regression** to real-world style prediction problems.

These projects helped me strengthen:
- data handling with **Pandas** and **NumPy**
- data visualization with **Matplotlib**
- model building using **Scikit-learn**
- train-test splitting
- interpreting model coefficients
- making predictions on new inputs
- evaluating regression model performance

The goal of this section is to move from theory to implementation by solving simple but practical prediction problems. 
The projects include delivery time prediction, laptop price estimation, and YouTube video performance forecasting. 

---

## Projects Included

### 1. Food Delivery Time Predictor
This project predicts **food delivery time** using:
- distance in kilometers
- preparation time in minutes

#### Objective
To understand how multiple input variables affect a continuous target variable using **multiple linear regression**.

#### What I did
- created a structured dataset with delivery-related variables
- explored the dataset using summary statistics
- visualized the relationship between distance, preparation time, and delivery time
- trained a linear regression model
- generated predictions on test data
- predicted delivery time for a new case

#### Example prediction
For a delivery with:
- **7 km distance**
- **15 minutes preparation time**

the model predicted a delivery time of approximately **37 minutes**. The notebook also reports a very high fit score on the sample data. 

---

### 2. Laptop Price Predictor
This project predicts **laptop price in INR** based on:
- RAM in GB
- storage in GB
- processor speed in GHz

#### Objective
To learn how hardware specifications influence laptop pricing and how regression can estimate a fair price.

#### What I did
- created a laptop specification dataset
- performed exploratory analysis and descriptive statistics
- visualized price relationships with RAM, storage, and processor speed
- trained a multiple linear regression model
- evaluated model predictions on test data
- estimated fair prices for new laptop configurations

#### Example predictions
- For a laptop with **16GB RAM, 512GB storage, and 3.2 GHz processor**, the predicted fair price was about **71,687 INR**.
- For a laptop with **8GB RAM, 512GB storage, and 2.8 GHz processor**, the model predicted a fair price close to **50,296 INR**. {index=7}

---

### 3. YouTube Video Performance Predictor
This project predicts **total views** based on:
- click-through rate (CTR)

#### Objective
To understand simple linear regression using a content-performance use case.

#### What I did
- created a CTR vs total views dataset
- explored the data statistically
- visualized the relationship between CTR and total views
- trained a simple linear regression model
- plotted the regression line
- predicted expected views for a new CTR value

#### Example prediction
For a video with **8% CTR**, the model predicted around **45,898 views**. The project also visualizes the regression line over the observed data. 

---

## Skills Practiced
Through these exercises, I practiced:
- regression modeling
- feature-target selection
- exploratory data analysis
- scatter plot visualization
- train-test split workflow
- prediction on unseen data
- interpreting coefficients and intercepts
- real-world style problem framing

---

## Tools & Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## Learning Outcomes
By completing these coding practice projects, I improved my ability to:
- translate a problem statement into an ML workflow
- prepare input features and target variables
- train and evaluate regression models
- interpret outputs in a practical context
- present machine learning work in a structured GitHub portfolio format

---

## Folder Structure
```text
Coding-Practice-Submission
│
├── Food Delivery Time Predictor.ipynb
├── Food Delivery Time Predictor.pdf
├── Laptop Price Predictor.ipynb
├── Laptop Price Predictor.pdf
├── YT Video Performance Predictor.ipynb
└── YT Video Performance Predictor.pdf
