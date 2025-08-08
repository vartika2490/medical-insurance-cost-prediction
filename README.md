#Medical Insurance Cost Prediction using Linear Regression
This project predicts individual medical insurance costs based on a number of personal attributes. It serves as a practical, end-to-end demonstration of a machine learning regression problem, from initial data exploration to model interpretation.

The model is built using Python and the Scikit-learn library, achieving an R-squared score of approximately 78% on the test data.

Table of Contents
.Project Overview

.Tech Stack

.Project Workflow

#Key Findings

How to Run

Project Overview
The goal of this project is to build a linear regression model that accurately predicts medical insurance charges. This involves understanding the relationships between a person's attributes (like age, BMI, and smoking status) and their medical expenses. The project demonstrates the entire data science workflow, making it a great example for anyone learning about regression analysis.

#The dataset used is the "Medical Cost Personal Datasets" from Kaggle.
.Tech Stack
.Python

Pandas: For data manipulation and analysis.
NumPy: For numerical operations.
Matplotlib & Seaborn: For data visualization and creating insightful plots.
Scikit-learn: For building and evaluating the machine learning model (LinearRegression, train_test_split, r2_score).

Project Workflow
Exploratory Data Analysis (EDA): The dataset was loaded, inspected for missing values, and analyzed to understand the distribution of the target variable (charges). Visualizations like histograms, box plots, and scatter plots were used to identify initial patterns and correlations.

Data Preprocessing: Categorical features (sex, smoker, region) were converted into a numerical format using one-hot encoding (pd.get_dummies) to make them suitable for the linear regression model.

Model Training: The dataset was split into training (80%) and testing (20%) sets. A LinearRegression model was then trained on the training data.
Model Evaluation: The trained model was evaluated on the unseen test data using the following metrics:

R-squared (R 
2
 ): To measure the proportion of variance explained by the model.

Mean Absolute Error (MAE): To understand the average prediction error in dollars.
Root Mean Squared Error (RMSE): To measure error while penalizing larger mistakes more heavily.
Interpretation: The model's coefficients were analyzed to determine the most significant factors influencing insurance costs.

Key Findings
The model explains approximately 78% of the variance in insurance charges (R 
2
approx0.78).

Smoking status is by far the most significant predictor. A smoker is predicted to have charges that are over $23,600 higher than a non-smoker, all other factors being equal.
Age and BMI are also strong positive predictors of cost. For every one-unit increase, charges are predicted to rise by ~$257 and ~$332, respectively.

How to Run
Clone the repository:

git clone https://github.com/your-username/medical-insurance-cost-prediction.git

Install the required libraries:

pip install pandas numpy matplotlib seaborn scikit-learn
Run the Jupyter Notebook or Python script to see the analysis and model training process.
