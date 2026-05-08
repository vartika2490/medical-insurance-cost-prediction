# Medical Insurance Cost Prediction using Linear Regression

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Tech Stack](#tech-stack)
- [Project Workflow](#project-workflow)
- [Exploratory Data Analysis](#1-exploratory-data-analysis-eda)
- [Data Preprocessing](#2-data-preprocessing)
- [Model Training](#3-model-training)
- [Model Evaluation](#4-model-evaluation)
- [Key Findings](#key-findings)
- [How to Run](#how-to-run)
- [Conclusion](#conclusion)

---

# Project Overview

Medical Insurance Cost Prediction is a machine learning project focused on predicting individual medical insurance expenses using Linear Regression. The project demonstrates a complete end-to-end machine learning workflow, including data analysis, preprocessing, model development, evaluation, and interpretation.

The primary objective is to understand how different personal and health-related factors influence medical insurance charges and to build a predictive model capable of estimating those costs with good accuracy.

Using Python and the Scikit-learn library, the model achieved an R² score of approximately **78%**, indicating strong predictive performance on unseen test data.

This project serves as a practical example for learning:
- Regression Analysis
- Data Preprocessing
- Feature Engineering
- Model Evaluation
- Data Visualization
- Machine Learning Fundamentals

---

# Dataset

The dataset used in this project is the **Medical Cost Personal Dataset** available on Kaggle.

The dataset contains demographic and health-related information, including:
- Age
- Gender
- BMI (Body Mass Index)
- Number of Children
- Smoking Status
- Region
- Medical Insurance Charges

The target variable for prediction is:
- **Insurance Charges**

---

# Tech Stack

## Programming Language
- Python

## Libraries Used

### Data Analysis & Processing
- Pandas
- NumPy

### Data Visualization
- Matplotlib
- Seaborn

### Machine Learning
- Scikit-learn

---

# Project Workflow

The project follows a structured machine learning pipeline:

1. Data Collection
2. Exploratory Data Analysis (EDA)
3. Data Cleaning & Preprocessing
4. Feature Encoding
5. Model Training
6. Model Evaluation
7. Result Interpretation

---

# 1. Exploratory Data Analysis (EDA)

Exploratory Data Analysis was performed to understand the dataset structure, identify patterns, and analyze relationships between variables.

The following analyses were conducted:
- Missing value inspection
- Statistical summary analysis
- Distribution analysis of insurance charges
- Correlation analysis
- Outlier detection
- Feature relationship visualization

Several visualizations were created using Matplotlib and Seaborn, including:
- Histograms
- Box Plots
- Scatter Plots
- Correlation Heatmaps

These visualizations helped identify important trends and influential factors affecting insurance costs.

---

# 2. Data Preprocessing

Before training the model, categorical features were converted into numerical form using **One-Hot Encoding (`pd.get_dummies`)**.

The following categorical columns were encoded:
- `sex`
- `smoker`
- `region`

This preprocessing step ensured compatibility with the Linear Regression algorithm.

Additional preprocessing included:
- Feature selection
- Data formatting
- Train-test splitting

---

# 3. Model Training

The dataset was divided into:
- **80% Training Data**
- **20% Testing Data**

A **Linear Regression** model from Scikit-learn was trained using the processed training dataset.

The model learned the relationships between input features and insurance charges to generate cost predictions.

---

# 4. Model Evaluation

The trained model was evaluated on unseen test data using multiple regression performance metrics.

## Evaluation Metrics

### R² Score
Measures how well the model explains the variance in insurance charges.

- Achieved R² Score: **~0.78**

### Mean Absolute Error (MAE)
Measures the average absolute difference between predicted and actual values.

### Root Mean Squared Error (RMSE)
Measures prediction error while giving higher penalties to larger errors.

The evaluation results indicate that the model performs effectively for a real-world regression problem.

---

# Key Findings

The analysis revealed several important insights:

- The model explains approximately **78%** of the variance in medical insurance charges.
- **Smoking status** is the strongest predictor of insurance expenses.
- Smokers are predicted to incur insurance costs that are more than **$23,600 higher** than non-smokers, keeping other variables constant.
- **Age** shows a strong positive correlation with insurance charges.
- **BMI** also significantly impacts medical costs.
- For every one-unit increase:
  - Insurance charges increase by approximately **$257** with age.
  - Insurance charges increase by approximately **$332** with BMI.

These findings highlight the strong influence of lifestyle and health-related attributes on medical insurance pricing.

---

# How to Run

## Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/medical-insurance-cost-prediction.git
